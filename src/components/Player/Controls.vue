<template>
	<div class="flex flex-col justify-center">
		<div class="flex justify-center items-center">
			<i class="fas fa-random text-base inline-block p-4"></i>
			<i class="fas fa-step-backward text-2xl inline-block p-2"></i>

			<button @click="isPlaying=!isPlaying" class="p-2" >
				<i v-if="!isPlaying" class="far fa-play-circle text-2xl inline-block"></i>
				<i v-else class="far fa-pause-circle text-2xl inline-block"></i>
			</button>

			<i class="fas fa-step-forward text-2xl inline-block p-2"></i>
			<img src="/img/repeat.svg" alt="repeat" class="h-5 ml-4">
		</div>

		<div class="flex justify-center items-center mt-1">
			<div class="text-xs text-gray-500">01:22</div>
			<div class="rounded-lg xl:w-200 bg-gray-500 h-1 ml-3 mr-3 w-64" />
			<div class="text-xs text-gray-500">02:32</div>
		</div>

	</div>
</template>

<script>
export default {

	data:()=>({
		isPlaying:false
	})

}
</script>

<style>

</style>