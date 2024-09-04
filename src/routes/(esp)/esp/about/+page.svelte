<script>
	import Pfp from '$lib/components/about/profile.svelte';
	import pfp1 from '$lib/images/pfps/Cory.jpg';
	import pfp2 from '$lib/images/pfps/Denny.jpg';
</script>

<!-- <svelte:head>
	<title>Quien somos</title>
	<meta name="description" content="Quien somos" />
</svelte:head> -->

<section class="text-column">
	<h1>Quien somos</h1>

	<div class="container">
		<Pfp
			img_src={pfp1}
			name="Cory Partridge"
			description="Soy profesora de inglés y tutora certificada TEFL, con 5 años de experiencia 
			enseñando el método NativeLinq. Soy originaria del Reino Unido, y completé tanto mi 
			Licenciatura en Español y Filosofía, como mi Maestría en la Universidad de Leeds. Soy 
			una ávida lectora, amante de la música y escritora, y también tengo amplia experiencia 
			trabajando con niños y jóvenes con Necesidades Educativas Especiales, como TDAH y Autismo, 
			proporcionándoles apoyo especializado 1:1."
		/>

		<Pfp
			img_src={pfp2}
			name="Denny Berndt"
			description="Soy originaria de Alemania y tengo una licenciatura en 
			Traducción Técnica y un máster por la Texas Tech University en Literatura 
			y Lengua Alemana con especialización en Literatura Española. Me he 
			especializado en la enseñanza de idiomas, la gestión de programas escolares 
			y educativos, así como en el desarrollo de planes de estudio para idiomas 
			y para niños con implantes cocleares colaborando con las instalaciones y 
			el personal de alto nivel del Centro Educativo Sada de Kuwait."
		/>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.container {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-content: center;
	}
</style>
