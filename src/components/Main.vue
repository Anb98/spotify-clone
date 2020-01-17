<template>
	<main class="bg-gray-800-spotify flex-1 overflow-y-auto" >
		<div class="px-8 pb-4">
			<h2 class="mt-20 text-4xl font-semibold ">Home</h2>
			<Section title='Recently Played' :albums='albums' />
			<Section title='Recently Played' :albums='albums' />
		</div>
	</main>
</template>

<script>
import Section from './Section';

export default {
	components:{
		Section,
	},
	data:()=>({
		albums:[
			{
				title:'Nada es imposible',
				src:'http://1.bp.blogspot.com/-Bpcb6Yf5axw/Uuvsp4f-v6I/AAAAAAAAWMA/X51UVkhp7_E/s1600/1511285_633509676711465_1822919331_n.jpg',
				description:'Nunca nada es imposible',
				followers:9876,
			},
			{
				title:'Nada es imposible',
				src:'http://1.bp.blogspot.com/-Bpcb6Yf5axw/Uuvsp4f-v6I/AAAAAAAAWMA/X51UVkhp7_E/s1600/1511285_633509676711465_1822919331_n.jpg',
				description:'Nunca nada es imposible',
				followers:9876,
			},
			{
				title:'Nada es imposible',
				src:'http://1.bp.blogspot.com/-Bpcb6Yf5axw/Uuvsp4f-v6I/AAAAAAAAWMA/X51UVkhp7_E/s1600/1511285_633509676711465_1822919331_n.jpg',
				description:'Nunca nada es imposible',
				followers:9876,
			},
			{
				title:'Nada es imposible',
				src:'http://1.bp.blogspot.com/-Bpcb6Yf5axw/Uuvsp4f-v6I/AAAAAAAAWMA/X51UVkhp7_E/s1600/1511285_633509676711465_1822919331_n.jpg',
				description:'Nunca nada es imposible',
				followers:9876,
			},
			{
				title:'Nada es imposible',
				src:'http://1.bp.blogspot.com/-Bpcb6Yf5axw/Uuvsp4f-v6I/AAAAAAAAWMA/X51UVkhp7_E/s1600/1511285_633509676711465_1822919331_n.jpg',
				description:'Nunca nada es imposible',
				followers:9876,
			},
		]
	})
}
</script>

<style>

</style>