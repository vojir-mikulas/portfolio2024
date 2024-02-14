<script lang="ts">
	export let isAvailable : boolean = false;
</script>

<div class="flex items-center gap-x-2 text-neutral-600 dark:text-neutral-400">
	<div class={`w-5 h-5 aspect-square rounded-full bg-opacity-40 dark:bg-opacity-30 flex items-center justify-center
	${isAvailable ? 'dark:bg-green-700 bg-green-500' : 'dark:bg-red-700 bg-red-500'}
	`}>
		<div class={`w-3 h-3 aspect-square rounded-full
		${isAvailable ? 'dark:bg-green-700 bg-green-500' : 'dark:bg-red-700 bg-red-500'}`}></div>
	</div>
	{#if isAvailable}
		<p>I am currently available for work.</p>
	{:else}
		<p>Currently not accepting any offers</p>
	{/if}
</div>
