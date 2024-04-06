<script>
	import Boxes from "$lib/components/boxes1.svelte";
	import leftLogo from "$lib/images/brand icons/i13.svg";
	import rightLogo from "$lib/images/brand icons/i14.svg";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<img src={leftLogo} alt="Left Logo" id="left-logo"/>

<section>

	<h1>
		Lo Que Ofrecemos
	</h1>

	<Boxes />

	<div class="info-box">
		<h1>Por Que Somos Distintos?</h1>
		<p>
			NativeLiq fue creado por dos profesores de Ingles, y creamos en el Metodo 
			Nativo. Aprender en el colegio ayudara solo hasta cierto punto, Para asegurar 
			el futuro de tu hijo/a en un mundo cada vez mas internacional, hace falta algo 
			mas. Con el metodo nativo, los ninos aprenden de la misma manera que los hablantes 
			nativos: hacia juegos, conversacion, y temas importantes para ellos.
		</p>
	</div>

	<div class="contact-button-container">
		<button>Contactar</button>
	</div>

</section>

<img src={rightLogo} alt="Right Logo" id="right-logo"/>

<style>
	section {
		position: relative;
		display: grid;
		justify-items: center;
		padding: 0px 25px;
		height: auto;
	}

	#left-logo {
		position: absolute;
		top: -100px;
		left: -450px;
		max-width: 600px;
		transform: scaleX(-1);
	}

	#right-logo {
		position: absolute;
		bottom: -200px;
		right: -300px;
		max-width: 550px;
		transform: rotate(30deg);
	}

	h1 {
		width: 100%;
		margin: 100px 0px 40px 0px;
	}

	.info-box {
		display: grid;
		max-width: 600px;
		margin: 50px 0px 0px 0px;
	}

	.contact-button-container {
		display: flex;
		justify-content: center;
		margin: 100px 0px;
	}

	button {
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
	}

	button:hover {
		background-color: var(--brand-color-3);
		color: white;
	}

	button:active {
		transform: scale(0.95);
	}

	@media (min-width: 0px) and (max-width: 1100px) {
		#left-logo, #right-logo {
			opacity: 0.2;
		}
	}
</style>
