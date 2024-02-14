<script>
	import Hero from './components/Hero.svelte';
	import AboutMe from './components/AboutMe.svelte';
	import Project from '$lib/components/Project.svelte';
	import WorkExperience from '$lib/components/WorkExperience.svelte';

</script>



<div class="flex flex-col h-full max-w-[40rem] mx-auto px-4">
	<Hero />
	<AboutMe/>
	<WorkExperience/>
	<div>
	 <Project title="naruto" imageUrl="/naruto.jpg"/>
	</div>
</div>

