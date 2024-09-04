<script>
	export let name = '';
	export let description = '';
	export let img_src = '';
</script>

<div class="container">
	<div class="top-wrapper">
		<div class="svg-background"></div>
		<div class="svg-background2"></div>
		<!-- <div class="circle"></div> -->
		<div class="pfp-container">
			<img class="profile" src={img_src} alt="Profile" />
		</div>
	</div>

	<div class="text-container">
		<p class="name-text">{name}</p>
		<p class="desc-text">{description}</p>
	</div>
</div>

<style>
	.container {
		position: relative;
		/* background-color: var(--brand-color-1); */
		/* background-color: #f9f9fa; */
		/* min-width: 280px; */
		/* min-height: 475px; */
		/* overflow: hidden; */
		/* box-shadow: 0px 0px 15px 1px rgb(179, 179, 179); */
		margin: 25px;
		height: auto;
		border-radius: 10px 10px 0px 0px;
	}

	.top-wrapper {
		position: relative;
		min-width: 280px;
		min-height: 475px;
		height: 200px;
		overflow: hidden;
		height: 200px;
		border-radius: 10px 10px 0px 0px;
		/* margin: 25px; */
	}

	.svg-background {
		width: 350%;
		height: 100%;
		position: absolute;
		top: -300px;
		left: -50px;
		z-index: 1;
		background-color: var(--brand-color-2);
		-webkit-clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
		clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
		transform: rotate(20deg);
		z-index: 2;
	}

	.svg-background2 {
		width: 100%;
		height: 100%;
		position: absolute;
		top: 0px;
		left: -70px;
		background-color: var(--brand-color-3);
		background-color: var(--brand-color-1);
		/* background-color: rgb(194, 194, 194); */
		z-index: 1;
		-webkit-clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
		clip-path: polygon(0 0, 14% 0, 48% 100%, 0% 100%);
		transform: rotate(40deg);
		z-index: 2;
	}

	.pfp-container {
		position: absolute;
		width: 150px;
		height: 150px;
		margin-top: -10px;
		margin-left: -10px;
		overflow: hidden;
		border-radius: 0px 50% 50% 0px;
		border: 7px solid #eceff1;
		z-index: 3;
	}

	.profile {
		width: 100%;
		height: auto;
		z-index: 3;
	}

	.text-container {
		/* background-color: #f9f9fa; */
		width: 100%;
		margin-top: -450px;
		padding-top: 170px;
		max-width: 250px;
		padding: 170px 25px 25px 35px;
		text-align: left;
		border-radius: 10px;
		box-shadow: 0px 0px 15px 1px rgb(179, 179, 179);
		z-index: 1;
	}

	.name-text {
		color: var(--brand-color-3);
		font-size: 28px;
		font-weight: 700;
		margin: 5px 0px 0px 0px;
		text-align: center;
	}

	.desc-text {
		font-size: 14px;
		margin: 15px 0px 0px 0px;
		max-width: 250px;
	}
</style>
