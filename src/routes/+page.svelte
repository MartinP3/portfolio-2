<script>
	import Hero from '../components/static/Hero.svelte';
	import AboutMe from '../components/static/AboutMe.svelte';
	import Portfolio from '../components/static/Portfolio.svelte';
	// @ts-ignore for some reason it doesn't like this import while I'm using font awesome  icons?
	import Contact from '../components/static/Contact.svelte';
	import MySkills from '../components/static/MySkills.svelte';
</script>

<svelte:head>
	<title>Martin Pedersen</title>
</svelte:head>
<div>
	<Hero />
	<AboutMe />
	<MySkills />
	<Portfolio />
	<Contact />
</div>

<style>
	* {
		scroll-behavior: smooth;
	}
</style>
