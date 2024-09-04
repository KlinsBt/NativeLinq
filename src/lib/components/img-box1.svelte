<script>
	export let title = '';
	export let text = '';
	export let imgSrc = '';
	export let imgAlt = '';
	export let imgAlignment = '';
</script>

<div class="info-box">
	<div style={imgAlignment === 'left' ? 'flex-direction: row-reverse;' : 'flex-direction: row;'}>
		<div>
			<h1>{title}</h1>
			<p>
				{text}
			</p>
		</div>
		<img src={imgSrc} alt={imgAlt} />
	</div>
</div>

<style>
	.info-box {
		display: grid;
		justify-items: center;
		background-color: white;
		width: 100%;
	}

	.info-box > div {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		width: 100%;
	}

	.info-box > div > div > h1 {
		max-width: 600px;
	}

	.info-box > div > div > p {
		max-width: 600px;
		padding: 0px 25px;
	}

	.info-box > div > img {
		width: 100%;
		height: auto;
	}

	@media (min-width: 1500px) {
		.info-box > div > img {
			max-width: 800px;
		}
	}

	@media (min-width: 1265px) and (max-width: 1499px) {
		.info-box > div > img {
			max-width: 600px;
		}
	}

	@media (min-width: 0px) and (max-width: 1264px) {
		.info-box > div {
			justify-content: center;
		}

		.info-box > div:nth-child(2) {
			flex-direction: column-reverse;
		}

		.info-box > div > div {
			align-self: center;
		}

		.info-box > div > img {
			max-width: 600px;
			align-self: center;
		}
	}
</style>
