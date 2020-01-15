<template>
	<div class="bg-gray-700-spotify w-screen text-red-100 h-20 px-5 flex justify-between items-center" >
		
		<Info/>
		<Controls/>
		<div></div>

	</div>
</template>

<script>
import Info from './Info';
import Controls from './Controls';

export default {
	components:{
		Info,
		Controls,
	}
}
</script>

<style>

</style>