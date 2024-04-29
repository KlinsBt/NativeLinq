<script>
	import Boxes from "$lib/components/boxes1.svelte";
	import leftLogo from "$lib/images/brand icons/i13.svg";
	import rightLogo from "$lib/images/brand icons/i14.svg";
	import Box1 from "$lib/components/infobox1.svelte";
	import LandingPage from "$lib/components/landingpage.svelte";
	import Box2 from "$lib/components/img-boxes1.svelte";
	import MainLogo from "/favicon.png";
</script>

<svelte:head>
	<title>NativeLinq</title>
    <meta name="description" 
	content="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. 
	Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a 
	en un mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos 
	aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas 
	importantes para ellos.">
	<meta name="keywords" content="nativeLinq, english, epanish, learning, children" />
	<meta name="author" content="NativeLinq" />
	<meta name="theme-color" content="#f9f9fa" />
	<link rel="icon" type="image/png" href="{MainLogo}" />

	<meta property="og:title" content="NativeLinq">
	<meta property="og:image" content="{MainLogo}">
	<meta property="og:type" content="website">
	<meta property="og:url" content="https://www.nativelinq.com/">
	<meta property="og:site_name" content="NativeLinq" />
	<meta property="og:description" 
	content="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. 
	Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a 
	en un mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos 
	aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas 
	importantes para ellos.">

</svelte:head>

<img src={leftLogo} alt="Left Logo" id="left-logo"/>

<section>

	<LandingPage />

	<h1>
		Lo Que Ofrecemos
	</h1>

	<Boxes />

	<div style="height: 50px;"></div>

	<Box2 />
	
	<Box1 />

	<div class="contact-button-container">
		<a href="mailto:hello@nativelinq.com">Contactar</a>
	</div>

</section>

<img src={rightLogo} alt="Right Logo" id="right-logo"/>

<style>
	section {
		position: relative;
		display: grid;
		justify-items: center;
		height: auto;
		background-color: #f9f9fa;
		width: 100%;
	}

	#left-logo {
		position: absolute;
		top: -100px;
		left: -450px;
		max-width: 600px;
		transform: scaleX(-1);
		z-index: 2;
	}

	#right-logo {
		position: absolute;
		bottom: -200px;
		right: -300px;
		max-width: 550px;
		transform: rotate(30deg);
	}

	section > h1 {
		width: 100%;
		margin: 100px 0px 40px 0px;
		padding: 0px 25px;
	}

	.contact-button-container {
		display: flex;
		justify-content: center;
		margin: 50px 0px;
		z-index: 2;
	}

	.contact-button-container > a {
		font-family: FigtreeExtraBold, "Segoe UI", "Helvetica Neue", sans-serif;
		font-size: 25px;
		text-align: center;
		color: var(--brand-color-3);
		transition: all 0.1s linear;
		background-color: #f0f0f000;
		border: 4px solid var(--brand-color-3);
		padding: 10px 20px;
		border-radius: 30px;
		cursor: pointer;
		text-transform: uppercase;
		text-decoration: none;
	}

	.contact-button-container > a:hover {
		background-color: var(--brand-color-3);
		color: white;
	}

	.contact-button-container > a:active {
		transform: scale(0.95);
	}

	@media (min-width: 0px) and (max-width: 1100px) {
		#left-logo, #right-logo {
			opacity: 0.2;
		}
	}
</style>
