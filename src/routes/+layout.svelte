<script>
	import "../app.css";
  import { fade } from 'svelte/transition';
  import Footer from '$lib/components/Footer.svelte';


  export let data;
</script>
<svelte:head>
 <title>Vojíř Mikuláš</title>
 <meta name="theme-color" content="var(--theme-bg)">
</svelte:head>

{#key data.pathname}
<main in:fade={{ duration: 100, delay: 110}} out:fade={{ duration: 100 }} class="min-h-full flex-1 flex flex-col dark:bg-neutral-900 dark:text-neutral-300 bg-white text-neutral-800">
 <slot></slot>
 <Footer/>
</main>
{/key}
