<script>
	export let title = '';
	export let text = '';
</script>

<div class="info-box">
	<h1>{title}</h1>
	<p>{text}</p>
</div>

<style>
	.info-box {
		display: grid;
		justify-items: center;
		padding: 50px 25px;
		background-color: white;
		width: 100%;
	}

	.info-box > h1 {
		max-width: 600px;
	}

	.info-box > p {
		max-width: 600px;
		padding: 0px 25px;
	}
</style>
