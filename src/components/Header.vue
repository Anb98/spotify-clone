<template>
	<header class="bg-gray-800-spotify py-2 flex justify-between" >
		<div class="flex justify-start items-center" >
			<button class="px-3" >
				<i class="fas fa-chevron-left"></i>
			</button>
			<button class="px-3" >
				<i class="fas fa-chevron-right"></i>
			</button>
			<div class="relative ml-1">
				<input type="text" class='text-xs text-gray-800 placeholder-gray-800 rounded-full pr-3 pt-1 pb-1 pl-7 ' placeholder="Buscar" >
				<i class="fas fa-search absolute left-0 pl-2 text-gray-800 text-sm" style='padding-top:0.35rem' ></i>
			</div>
		</div>

		<div class="px-4" >
			<a href="#" class="hover:underline">
				<i class="far fa-user-circle pr-2"></i>
				<span class="text-sm mr-2" >Username last</span>
			</a>
			<button>
				<i class="fas fa-chevron-down px-2 text-sm"></i>
			</button>
		</div>
	</header>
</template>

<script>
export default {

}
</script>

<style>

</style>