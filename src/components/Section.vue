<template>
	<section class="mt-12">
		<h3 class="font-semibold text-xl border-b border-gray-900 pb-2 ">Recently Played</h3>
		<div class="flex items-center mt-4 -mx-4 flex-wrap ">
			
			<a v-for="(album, i) of albums" :key='i' href="#" class=" w-1/5 px-4">
				<img :src="album.src" alt="cover album">
				<div class="hover:underline">{{album.title}}</div>
				<div class="text-gray-500 mt-1">{{album.description}}</div>
				<div class="uppercase text-xs text-gray-500 mt-1">{{album.followers}} Followers</div>
			</a>

		</div>
	</section>
</template>

<script>
export default {
	props:{
		title:{ type:String, required:true },
		albums:{ type:Array, required:true }
	}
}
</script>

<style>

</style>