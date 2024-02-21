<script lang="ts">
	export let title : string = "";
	export let imageUrl :string = "";
</script>

<a href="/projects/placeholder" class="group flex flex-col w-full aspect-video transition-colors
dark:hover:bg-neutral-800 dark:bg-neutral-850 hover:bg-neutral-100 bg-white
dark:border dark:border-neutral-800
rounded-xl drop-shadow-md overflow-hidden p-2">
	<h4 class="mb-2 dark:text-neutral-300 text-neutral-800">{title}</h4>
	<div class="bg-neutral-900 rounded-md overflow-hidden">
		<img class="w-full h-full object-cover group-hover:scale-105 transition-transform  duration-300" src={imageUrl} alt="preview">
	</div>
</a>

<style>

</style>