<script>
	import "../app.css";
  import Footer from '$lib/components/Footer.svelte';
  import Navbar from '$lib/components/Navbar.svelte';


</script>
<svelte:head>
 <title>Vojíř Mikuláš</title>
 <meta name="theme-color" content="var(--theme-bg)">
</svelte:head>

<main  class="min-h-full flex-1 flex flex-col dark:bg-neutral-900 dark:text-neutral-300 bg-white text-neutral-800 py-8">
 <slot></slot>
 <Footer/>
</main>
<Navbar></Navbar>
