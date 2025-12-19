<script>
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Header from '../components/Header.svelte';
	import Hero from '../components/Hero.svelte';
	import Divider from '../components/Divider.svelte';
	import Story from '../components/Story.svelte';
	import Craft from '../components/Craft.svelte';
	import Shop from '../components/Shop.svelte';
	import Footer from '../components/Footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}

<main class="page-container">
	<section class="pattern">
		<Header />
		<Hero />
		<Divider />
	</section>
	<Story/>
	<Craft/>
	<Shop/>
	<Footer/>
</main>
