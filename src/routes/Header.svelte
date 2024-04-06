<script>
	import logo from "$lib/images/brand icons/i8.svg";
</script>

<header>
	<nav>
		<a href="/" id="logo-container">
			<img src={logo} alt="Logo" />
		</a>
		<ul>
			<li>
				<a href="/">Contactar</a>
			</li>
			<li>
				<a href="/">FAQs</a>
			</li>
			<li>
				<a href="/">Quien somos</a>
			</li>
		</ul>
	</nav>
</header>

<style>

	header {
		display: flex;
		justify-content: space-between;
		width: 100%;
	}

	nav {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		width: 100%;
		padding: 5% 7% 0px 7%;
	}

	#logo-container {
		width: 240px;
		height: auto;
	}

	#logo-container > img {
		width: 100%;
		height: 100%;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--brand-color-3);
		font-weight: 700;
		font-size: 15px;
		/* text-transform: uppercase; */
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--brand-color-2);
	}
</style>
