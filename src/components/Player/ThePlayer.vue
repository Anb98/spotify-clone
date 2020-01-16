<template>
	<div class="bg-gray-700-spotify w-screen text-red-100 h-20 px-5 flex justify-between items-center" >
		
		<Info/>
		<Controls/>
		<Volume/>

	</div>
</template>

<script>
import Info from './Info';
import Controls from './Controls';
import Volume from './Volume';

export default {
	components:{
		Info,
		Controls,
		Volume,
	}
}
</script>

<style>

</style>