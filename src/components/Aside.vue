<template>
	<aside class="bg-gray-900-spotify w-48 flex-none flex flex-col">
		<header>
			<ul>
				<li 
					:class="[selected==='home' ? 'border-l-2 border-green-600 font-bold' : 'font-semibold', 'py-2 pl-2', 'cursor-pointer hover:text-white']"
					@click="selected='home'"
				>
					<a>
						<i class="fas fa-home"></i>
						<span class="ml-2">Home</span>
					</a>
				</li>
				<li 
					:class="[selected==='search' ? 'border-l-2 border-green-600 font-bold' : 'font-semibold', 'py-2 pl-2', 'cursor-pointer hover:text-white']"
					@click="selected='search'"
				>
					<a>
						<i class="fas fa-search"></i>
						<span class="ml-2">Search</span>
					</a>
				</li>
				<li 
					:class="[selected==='radio' ? 'border-l-2 border-green-600 font-bold' : 'font-semibold', 'py-2 pl-2', 'cursor-pointer hover:text-white']"
					@click="selected='radio'"
				>
					<a>
						<i class="fas fa-broadcast-tower"></i>
						<span class="ml-2">Radio</span>
					</a>
				</li>
			</ul>
		</header>
		<div class="overflow-y-auto mt-2 px-5">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus placeat quasi eaque expedita consectetur beatae inventore distinctio fugit perferendis temporibus nemo, vel, sapiente nesciunt fugiat ut voluptas voluptatum quis nulla. Harum commodi similique illo! Molestias deleniti voluptas amet optio cupiditate eveniet molestiae, nemo debitis doloremque nisi pariatur at est placeat eum tempore ratione atque aut obcaecati assumenda dolores rem maxime nostrum dolorum dolorem. Est non at mollitia minus commodi! Reiciendis dolorem, corrupti odit aut, inventore deserunt quia quidem enim voluptatum ratione aperiam nam molestias non illum obcaecati quasi harum nesciunt? Totam autem beatae aliquid officiis accusantium temporibus, asperiores corrupti ipsum et nostrum sapiente expedita, distinctio nesciunt, magnam a corporis facilis assumenda. Culpa, sunt magni? Eum corporis maiores eius repudiandae, voluptatum quae pariatur, veniam, velit cupiditate minima eaque. Dignissimos praesentium quis culpa ipsam voluptate autem fugit architecto obcaecati sed consequuntur a commodi laboriosam, aliquam magnam libero mollitia nisi tempore amet sequi at quas, incidunt ut asperiores. Eaque quae nihil nostrum quod nisi in laboriosam ut, a sit numquam quia, at similique ex rerum! A voluptatum perferendis consectetur quaerat sunt corporis illum vel enim vero pariatur veniam esse voluptatibus quis cupiditate, beatae placeat, aut iure quo natus quam odio mollitia temporibus harum debitis? Sit impedit possimus iure mollitia perferendis aliquam, asperiores maiores, repellat itaque minus fuga vitae. Nobis officiis iste incidunt sit autem esse deserunt, maiores eum ratione, natus quia harum dolorum beatae ipsum ipsa adipisci magni quidem inventore tenetur vel? Sint sequi consequuntur at dignissimos odio commodi facilis! Ipsa, mollitia velit.
		</div>
		<footer class="p-4">
			<a href="#" >
				<span 
					class="inline-block rounded-full border-gray-400 border-2 w-8 h-8 text-center mr-2"
					style="padding-top: 0.1em"
				>
					<i class="fas fa-plus"></i>
				</span>
				<span>New playlist</span>
			</a>
		</footer>
	</aside>
</template>

<script>
export default {
	data:()=>({
		selected:'home'
	}),
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