<template>
	<div class="mt-4" >
		<h3 class="text-xs font-normal tracking-widest text-gray-500 uppercase" >{{title}}</h3>
		<ul>
			<li class="truncate" v-for="(el, i) of items" :key='i' >
				<a v-if="typeof el === 'string'" href="#" class="hover:text-white">{{el}}</a>
				<a v-else href="#" class="hover:text-white">{{el.name}}</a>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	props:{
		title:{ required:true, type:String },
		items:{ required:true, type: Array }
	}

}
</script>

<style>

</style>