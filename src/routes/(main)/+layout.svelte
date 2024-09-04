<script>
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	import '../styles.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<Footer />
</div>

<style>
	.app {
		display: grid;
		justify-items: center;
		min-height: 100vh;
		width: 100%;
	}

	main {
		position: relative;
		width: 100%;
		display: grid;
		justify-items: center;
		overflow: hidden;
	}
</style>
