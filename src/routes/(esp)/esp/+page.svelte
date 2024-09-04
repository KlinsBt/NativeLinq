<script>
	import Boxes from '$lib/components/boxes1.svelte';
	import leftLogo from '$lib/images/brand icons/i13.svg';
	import rightLogo from '$lib/images/brand icons/i14.svg';
	import LandingPage from '$lib/components/landingpage.svelte';
	import img1 from '$lib/images/bgs/img1.jpg';
	import img2 from '$lib/images/bgs/img2.jpg';
	// import img3 from '$lib/images/bgs/img3.jpg';
	import ImgBox from '$lib/components/img-box1.svelte';
	import InfoBox from '$lib/components/infobox1.svelte';
	// import MainLogo from "/favicon.png";
</script>

<svelte:head>
	<title>NativeLinq</title>
	<meta
		name="description"
		content="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. 
		Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a 
		en un mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos 
		aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas 
		importantes para ellos."
	/>
	<meta name="keywords" content="nativeLinq, ingles, español, aprender, niños" />
	<!-- <meta name="author" content="NativeLinq" /> -->
	<meta name="theme-color" content="#f9f9fa" />
	<link rel="icon" type="image/png" href="/favicon.png" />

	<meta property="og:title" content="NativeLinq" />
	<meta property="og:image" content="/favicon.png" />
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://www.nativelinq.com/" />
	<meta property="og:site_name" content="NativeLinq" />
	<meta
		property="og:description"
		content="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. 
		Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a 
		en un mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos 
		aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas 
		importantes para ellos."
	/>

	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://www.nativelinq.com/" />
	<meta property="twitter:title" content="NativeLinq" />
	<meta
		property="twitter:description"
		content="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. 
		Aprender en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a 
		en un mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos 
		aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas 
		importantes para ellos."
	/>
	<meta property="twitter:image" content="/favicon.png" />
</svelte:head>

<img src={leftLogo} alt="Left Logo" id="left-logo" />

<section>
	<LandingPage title="APRENDE INGLÉS" />

	<h1>Lo Que Ofrecemos</h1>

	<Boxes
		box_title_1="Aprendizaje Divertido"
		box_text_1="En NativeLinq creemos que aprender Ingles debe ser divertido. Nuestros profesores 
		tienen mucha energia y hacen juegos divertidos en Ingles para reforzar las habilidades de 
		hablar de tu hijo."
		box_title_2="Preparacion De Examenes"
		box_text_2="Preparacion experta para cualquier examen: de A1 hasta C2. Aprende con los mejores 
		profesores y asegure tu futuro."
		box_title_3="Metodo Nativo"
		box_text_3="Aprender como aprenden los nativos: sin libros de texto ni ejercicios de gramática. 
		Aprender Ingles util y practico, hacia clases de conversacion con hablantes nativos."
	/>

	<div style="height: 50px;"></div>

	<ImgBox
		title="Nuestra Misión"
		text="En NativeLinq, nuestra misión es clara: ofrecer una educación en inglés de la más alta calidad, 
		personalizada para estudiantes de todas las edades y niveles. Con más de cinco años de experiencia 
		enseñando en Europa, el norte de África y en línea, hemos visto de primera mano cómo aprender un 
		nuevo idioma puede transformar vidas."
		imgSrc={img1}
		imgAlt="Kid"
	/>

	<ImgBox
		title="Nuestra Visión"
		text="Creemos firmemente que dominar un idioma es la clave para abrir un mundo de oportunidades. 
		Por eso, en NativeLinq, nos dedicamos a equipar a nuestros estudiantes con las habilidades lingüísticas 
		que necesitan para sentirse confiados y preparados para su futuro."
		imgSrc={img2}
		imgAlt="Kid"
		imgAlignment="left"
	/>

	<InfoBox
		title="Por Que Somos Distintos?"
		text="NativeLinq fue creado por dos profesores de Ingles, y creamos en el Metodo Nativo. Aprender
		en el colegio ayudara solo hasta cierto punto. Para asegurar el futuro de tu hijo/a en un
		mundo cada vez mas internacional, hace falta algo mas. Con el metodo nativo, los ninos
		aprenden de la misma manera que los hablantes nativos: hacia juegos, conversacion, y temas
		importantes para ellos."
	/>

	<div class="contact-button-container">
		<a href="mailto:hello@nativelinq.com">Contactar</a>
	</div>
</section>

<img src={rightLogo} alt="Right Logo" id="right-logo" />

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
		font-family: FigtreeExtraBold, 'Segoe UI', 'Helvetica Neue', sans-serif;
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
		#left-logo,
		#right-logo {
			opacity: 0.2;
		}
	}
</style>
