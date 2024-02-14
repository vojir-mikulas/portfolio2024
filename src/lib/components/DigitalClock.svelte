<script lang="ts">
	//display current time in paragraph
	import { onMount } from 'svelte';

	let time: Date = new Date();

	$: hours = time.getHours().toString().padStart(2, '0');;
	$: minutes = time.getMinutes().toString().padStart(2, '0');;
	$: seconds = time.getSeconds().toString().padStart(2, '0');;

	onMount(() => {
		const interval = setInterval(() => {
			time = new Date();
		}, 1000);

		return () => {
			clearInterval(interval);
		};
	});
</script>

<p {...$$props}>
	{#if time}
		{hours}:{minutes}:{seconds}
	{:else}
		ERR:ERR
	{/if}
</p>