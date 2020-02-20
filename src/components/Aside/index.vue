<template>
	<aside class="bg-gray-900-spotify w-48 flex-none flex flex-col justify-between">
		<header>
			<ul>
				<li
					v-for="(item, i) of headerItems"
					:key='i'
					:class="[selected===item.name ? 'border-l-2 border-green-600 font-bold' : 'font-semibold', 'py-2 pl-2', 'cursor-pointer hover:text-white']"
					@click="selected=item.name"
				>
					<a>
						<i :class="['fas', item.icon]"></i>
						<span class="ml-2">{{item.name}}</span>
					</a>
				</li>
			</ul>
		</header>

		<div class="overflow-y-auto mt-2 px-5">
			<List title='Your library' :items='yourLibrary' />
			<List title='Playlists' :items='playlists' />
		</div>
		
		<footer class="border-t border-gray-800 px-4 py-2 hover:text-white">
			<a href="#" >
				<span 
					class="inline-block rounded-full border-gray-400 border w-6 h-6 text-center mr-2 text-xs">
					<i class="fas fa-plus text-sm pt-1"></i>
				</span>
				<span>New playlist</span>
			</a>
		</footer>
	</aside>
</template>

<script>
import List from './List';

export default {
	components:{
		List
	},
	async mounted(){
		try {
			const res = await fetch('https://api.spotify.com/v1/browse/featured-playlists?limit=20&country=us&locale=es',{
				headers:{ Authorization: `Bearer ${process.env.VUE_APP_BEARER_TOKEN}`},
			});
	
			const data = await res.json();
			this.transformData(data.playlists.items);
		} catch (error) {
			// console.log('error :', error);
		}
	},
	data:()=>({
		selected:'Home',
		headerItems: [ 
			{name:'Home', icon: 'fa-home'},
			{name:'Search', icon: 'fa-search'},
			{name:'Radio', icon: 'fa-broadcast-tower'},
		],
		yourLibrary: [ 'Made for you', 'Recently player', 'Liked songs', 'Albums', 'Artists', 'Podcast' ],
		playlists: []

	}),
	methods:{
		transformData(playlists){
			for (const item of playlists)
				this.playlists.push({
					id: item.id,
					name:item.name, 
					tracks: item.tracks.href
				});
		}
	}
}
</script>

<style>
::-webkit-scrollbar{
	width: 8px;
	background: #121212;
}

::-webkit-scrollbar-thumb{
	background: #535353;
	border-radius: 8px;
}


</style>