<script>
	import DigitalClock from '$lib/components/DigitalClock.svelte';
	import Availability from '$lib/components/Availability.svelte';
</script>

<section class="items-center flex flex-col gap-y-5 my-5 sm:text-center">
	<div class="">
		<DigitalClock class="dark:text-neutral-600 text-neutral-300"/>
	</div>
	<div class="h-40 w-40 rounded-full overflow-hidden">
		<img class="w-full h-full object-cover aspect-square" src="/avatar.jpeg" alt="avatar">
	</div>
	<div class="sm:w-fit w-full text-center sm:text-left">
		<h1 class="text-5xl font-bold sm:text-8xl">Mikuláš Vojíř</h1>
		<h2 class="sm:text-4xl text-3xl font-bold mt-1 dark:text-neutral-500 text-neutral-700">Fullstack developer</h2>
		<div class="flex flex-col sm:flex-row justify-between mt-2 sm:mt-6 dark:text-neutral-700 text-neutral-400 text-sm">
			<p>Based in Prague, Czech Republic</p>
			<p class="">Powered by Appraising</p>
		</div>
	</div>

	<div>
		<Availability/>
	</div>
</section>