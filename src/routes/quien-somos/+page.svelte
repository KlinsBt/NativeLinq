<script>
	import Pfp from "$lib/components/profile.svelte";
	import pfp1 from "$lib/images/pfps/Cory.jpg";
	import pfp2 from "$lib/images/pfps/Denny.jpg";

</script>





<svelte:head>
	<title>Quien somos</title>
	<meta name="description" content="Quien somos" />
</svelte:head>

<section class="text-column">
	<h1>Quien somos</h1>

	<div class="container">
		<Pfp
		img_src={pfp1}
		name="Cory Partridge" 
		description="I'm a TEFL certified English teacher and tutor, 
		with 5 years of experience teaching the NativeLinq method. 
		I'm originally from the UK, and I created NativeLinq to deliver 
		personalised English learning to students at the highest quality. 
		I'm an avid reader, music lover, and writer!"/>
	
		<Pfp 
		img_src={pfp2}
		name="Denny Berndt" 
		description="I am originally from Germany and have a B.A. in Technical Translation and an M.A. 
		from Texas Tech University in German Literature & Language with a minor in Spanish 
		Literature. I have specialized in language education, school and education program 
		management as well as curriculum development for language and for children with 
		cochlear implants collaborating with the high-end facilities and staff at Sada 
		Educational Center in Kuwait."/>
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