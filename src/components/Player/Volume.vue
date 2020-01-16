<template>
	<div class="flex items-center">
		<button>
			<svg class="fill-current text-gray-400 hover:text-white h-6 w-6" width="24" height="24" viewBox="0 0 24 24"><path d="M0 0h24v24H0z" fill="none"/><path d="M15 6H3v2h12V6zm0 4H3v2h12v-2zM3 16h8v-2H3v2zM17 6v8.18c-.31-.11-.65-.18-1-.18-1.66 0-3 1.34-3 3s1.34 3 3 3 3-1.34 3-3V8h3V6h-5z"/></svg>
		</button>
		<button class="ml-2">
			<svg class="fill-current text-gray-400 hover:text-white h-5 w-5" width="24" height="24" viewBox="0 0 24 24"><path fill="none" d="M0 0h24v24H0z"/><path d="M3 6h18V4H3c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h4v-2H3V6zm10 6H9v1.78c-.61.55-1 1.33-1 2.22s.39 1.67 1 2.22V20h4v-1.78c.61-.55 1-1.34 1-2.22s-.39-1.67-1-2.22V12zm-2 5.5c-.83 0-1.5-.67-1.5-1.5s.67-1.5 1.5-1.5 1.5.67 1.5 1.5-.67 1.5-1.5 1.5zM22 8h-6c-.5 0-1 .5-1 1v10c0 .5.5 1 1 1h6c.5 0 1-.5 1-1V9c0-.5-.5-1-1-1zm-1 10h-4v-8h4v8z"/></svg>
		</button>
		<a href="#" class="ml-2 text-gray-400" @click="hasVolume=!hasVolume" >
			<i v-if="hasVolume" class="fas fa-volume-up"></i>
			<i v-else class="fas fa-volume-mute"></i>
		</a>
        <div class="bg-gray-500 rounded-lg w-20 h-1 ml-3"></div>
        <button class="ml-4">
			<svg class="fill-current text-gray-400 hover:text-white h-4 w-4" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M15 3h6v6M9 21H3v-6M21 3l-7 7M3 21l7-7"/></svg>
        </button>

	</div>
</template>

<script>
export default {
	data:()=>({
		hasVolume:true
	})
}
</script>

<style>

</style>