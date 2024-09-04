<script>
	import Boxes from '$lib/components/boxes1.svelte';
	import leftLogo from '$lib/images/brand icons/i13.svg';
	import rightLogo from '$lib/images/brand icons/i14.svg';
	import LandingPage from '$lib/components/landingpage.svelte';
	import img1 from '$lib/images/bgs/img1.jpg';
	import img2 from '$lib/images/bgs/img2.jpg';
	import img3 from '$lib/images/bgs/img3.jpg';
	import ImgBox from '$lib/components/img-box1.svelte';
	import InfoBox from '$lib/components/infobox1.svelte';
	// import MainLogo from "/favicon.png";
</script>

<svelte:head>
	<title>NativeLinq</title>
	<meta
		name="description"
		content="NativeLinq was created by two English teachers, and we believe in the Native Method. 
		Learning at school will only help to a certain extent. To secure your child's future in an 
		increasingly international world, something more is needed. With the native method, children 
		learn in the same way as native speakers: through games, conversation, and topics that are 
		important to them. important to them."
	/>
	<meta name="keywords" content="nativeLinq, english, epanish, learning, children" />
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
		content="NativeLinq was created by two English teachers, and we believe in the Native Method. 
		Learning at school will only help to a certain extent. To secure your child's future in an 
		increasingly international world, something more is needed. With the native method, children 
		learn in the same way as native speakers: through games, conversation, and topics that are 
		important to them. important to them."
	/>

	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://www.nativelinq.com/" />
	<meta property="twitter:title" content="NativeLinq" />
	<meta
		property="twitter:description"
		content="NativeLinq was created by two English teachers, and we believe in the Native Method. 
		Learning at school will only help to a certain extent. To secure your child's future in an 
		increasingly international world, something more is needed. With the native method, children 
		learn in the same way as native speakers: through games, conversation, and topics that are 
		important to them. important to them."
	/>
	<meta property="twitter:image" content="/favicon.png" />
</svelte:head>

<img src={leftLogo} alt="Left Logo" id="left-logo" />

<section>
	<LandingPage title="LEARN ENGLISH" />

	<h1>What We Offer</h1>

	<Boxes
		box_title_1="Fun Learning"
		box_text_1="At NativeLinq we believe that learning English should be fun. Our teachers 
		are energetic and play fun games in English to reinforce your child's speaking skills."
		box_title_2="Exam Preparation"
		box_text_2="Expert preparation for any exam: from A1 to C2. Learn with the best 
		teachers and secure your future."
		box_title_3="Native Method"
		box_text_3="Learn the way native speakers learn: without textbooks or grammar exercises. 
		Learn English in a practical and useful way, through conversation classes with native speakers."
	/>

	<div style="height: 50px;"></div>

	<ImgBox
		title="Our Mission"
		text="At NativeLinq, our mission is clear: to provide the highest quality English education, 
		personalized for students of all ages and levels. With over five years of experience teaching 
		across Europe, North Africa, and online, we’ve seen firsthand how learning a new language can 
		transform lives. "
		imgSrc={img1}
		imgAlt="Kid"
	/>

	<ImgBox
		title="Our Vision"
		text="We firmly believe that mastering a language is the key to unlocking a world of opportunities. 
		That’s why at NativeLinq, we’re dedicated to equipping our students with the language skills they 
		need to feel confident and prepared for their future."
		imgSrc={img2}
		imgAlt="Kid"
		imgAlignment="left"
	/>

	<InfoBox
		title="Why Are We Different?"
		text="NativeLinq was created by two English teachers, and we believe in the Native Method. 
		Learning at school will only help to a certain extent. To secure your child's future in an 
		increasingly international world, something more is needed. With the native method, children 
		learn in the same way as native speakers: through games, conversation, and topics that are 
		important to them."
	/>

	<div class="contact-button-container">
		<a href="mailto:hello@nativelinq.com">Contact</a>
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
