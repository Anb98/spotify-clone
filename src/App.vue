<template>
	<div id="app" class="flex flex-col h-screen text-gray-400" >
		<div class="flex flex-1 overflow-y-hidden" >
			<Aside/>
			<div class="flex flex-col w-full">
				<Header/>
				<Main/>
			</div>
		</div>
		<Player/>
	</div>
</template>

<script>
import Header from './components/Header';
import Aside from './components/Aside/index';
import Main from './components/Main';
import Player from './components/Player/ThePlayer';

export default {
  name: 'app',
  components: {
	Header,
	Aside,
	Main,
	Player
  }
}
</script>

<style>
@import 'assets/styles/tailwind.postcss';

</style>
