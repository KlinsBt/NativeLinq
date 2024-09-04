<script>
	// @ts-nocheck
	import icon1 from '$lib/images/libro-abierto2.png';
	import icon2 from '$lib/images/chat.png';
	import icon3 from '$lib/images/usuarios.png';

	export let box_title_1 = '';
	export let box_text_1 = '';
	export let box_title_2 = '';
	export let box_text_2 = '';
	export let box_title_3 = '';
	export let box_text_3 = '';
</script>

<div class="boxes-container">
	<div class="box">
		<div class="box-img-container">
			<img src={icon1} alt="Box Icon" />
		</div>
		<h2>{box_title_1}</h2>
		<p>{box_text_1}</p>
	</div>
	<div class="box">
		<div class="box-img-container">
			<img src={icon2} alt="Box Icon" />
		</div>
		<h2>{box_title_2}</h2>
		<p>{box_text_2}</p>
	</div>
	<div class="box">
		<div class="box-img-container">
			<img src={icon3} alt="Box Icon" />
		</div>
		<h2>{box_title_3}</h2>
		<p>{box_text_3}</p>
	</div>
</div>

<style>
	.boxes-container {
		display: flex;
		justify-content: center;
		align-items: start;
		flex-wrap: wrap;
		gap: 1rem;
		height: auto;
	}

	.box {
		display: flex;
		flex-direction: column;
		justify-content: start;
		align-items: center;
		gap: 1rem;
		padding: 1rem;
		border: 1px solid rgba(0, 0, 0, 0);
		border-radius: 10px;
		max-width: 220px;
		height: 350px;
		transition: all 0.1s linear;
		/* cursor: pointer; */
	}

	.box:hover {
		border: 1px solid var(--brand-color-3);
	}

	.box:nth-child(1) > .box-img-container {
		background-color: rgba(252, 130, 89);
	}

	.box:nth-child(2) > .box-img-container {
		background-color: rgb(255 238 156);
	}

	.box:nth-child(3) > .box-img-container {
		background-color: rgb(98 93 238);
	}

	.box-img-container {
		width: 100px;
		height: 100px;
		display: flex;
		justify-content: center;
		align-items: center;
		border-radius: 25px;
	}

	.box-img-container > img {
		width: 70%;
		height: auto;
		object-fit: contain;
	}

	.box > h2 {
		text-align: center;
		max-width: 155px;
		margin: 5px 0px 0px 0px;
	}

	.box > p {
		text-align: center;
		margin: 5px 0px 0px 0px;
	}
</style>
