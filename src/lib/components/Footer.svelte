<script lang="ts">
	let date: Date = new Date();
	let thisYear: number = date.getFullYear();
</script>
<footer class="w-full flex flex-col gap-y-4 items-center justify-center mt-auto p-4 text-center">
	<div>
		<ul class="flex gap-x-5 items-center">
			<li class="hover:scale-110 transition-transform"><a href="#Github"><img src="" alt="Github"></a></li>
			<li class="hover:scale-110 transition-transform"><a href="#LinkedIn"><img src="" alt="LinkedIn"></a></li>
			<li class="hover:scale-110 transition-transform"><a href="#StartUp_Jobs"><img src="" alt="StartUp Jobs"></a></li>
			<li class="hover:scale-110 transition-transform"><a href="#StackOverflow"><img src="" alt="StackOverflow"></a>
			</li>
		</ul>
	</div>
	<div>
		<p class="dark:text-neutral-700 text-neutral-400">Copyright
			&copy {2024 === thisYear ? thisYear : `2024 - ${date.getFullYear()}` } Vojíř</p>
	</div>
</footer>