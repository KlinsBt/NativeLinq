<script>
	// @ts-nocheck
	import logo from '$lib/images/brand icons/i17.png';
	import l from '$lib/i18-strings/lang.json';
	import { goto } from '$app/navigation';

	let lang = l['esp'];
	let selected = '/esp';

	function changeLanguage(langStr) {
		goto(selected);
	}
</script>

<header>
	<nav>
		<a href="/esp" id="logo-container">
			<img src={logo} alt="Logo" />
		</a>
		<ul>
			<li>
				<a href="mailto:hello@nativelinq.com">{lang.header.link1}</a>
			</li>
			<li>
				<a href="/esp/about">{lang.header.link2}</a>
			</li>
			<select
				name="/esp"
				id="select-lang"
				bind:value={selected}
				on:change={() => changeLanguage(selected)}
			>
				<option value="/">Ingles</option>
				<option value="/esp">Español</option>
			</select>
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
		padding: 20px 7% 2% 7%;
	}

	#logo-container {
		width: 240px;
		height: auto;
	}

	#logo-container > img {
		width: 100%;
		height: auto;
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

	#select-lang {
		background-color: var(--brand-color-3);
		border-radius: 10px;
		border: 4px solid var(--brand-color-2);
		color: var(--brand-color-1);
		font-weight: 600;
		font-size: 12px;
		letter-spacing: 0.1em;
		text-transform: uppercase;
		padding: 5px;
		cursor: pointer;
	}

	#select-lang:hover {
		border: 4px solid var(--brand-color-1);
	}
</style>
