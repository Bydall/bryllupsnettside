<script lang="ts">
	import { resolve } from '$app/paths';
	import { page } from '$app/state';

	export let open: boolean;
	export let toggleMenu: () => void;
	export let closeMenu: () => void;

</script>

<header>
	
	<nav>

	<button class="hamburger" on:click={toggleMenu}>
		{#if open}
		 ✕
		{:else}
		  ☰
		{/if}
	</button>

	 <div class:active={open} class="links">
		<ul>
			<li aria-current={page.url.pathname === '/' ? 'page' : undefined}>
				<a href="#mainpage" on:click={closeMenu}>Hjem</a>
			</li>
			<li aria-current={page.url.pathname === '/program' ? 'page' : undefined}>
				<a href="#Program" on:click={closeMenu}>Program</a>
			</li>
			<li aria-current={page.url.pathname === '/praktisk' ? 'page' : undefined}>
				<a href="#Praktisk" on:click={closeMenu}>Praktisk Info</a>
			</li>
			<li aria-current={page.url.pathname === '/onskeliste' ? 'page' : undefined}>
				<a href="#Onskeliste" on:click={closeMenu}>Ønskelister</a>
			</li>
		</ul>
	</div>	
	
		
	<div class:shifted={open} class="middle">
		<a href={resolve('/')}>
		Mathilde og Håvard
		</a>
	</div>

	<div>
		<i class="fa-solid fa-plus" aria-hidden="true"></i>
	</div>

	</nav>

	
</header>

<style>
	header {
		
		padding: 1rem;
		display: block;
		
		
	}

	.middle {
		margin: auto;
	}

	.middle a {
		font-family: 'Waterfall';
		font-weight:normal;
    	font-size: 2.2rem;
    	text-decoration: none;
		text-transform: none;
	}

	.links{
		display: block;
	}

	.links a{
		font-family: 'Klee 1';
	}

	
	nav {
		display: flex;
		align-items: center;
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
	
	
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
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
		color: var(--color-text);
		font-family: 'Cookie';
		font-weight: normal;
		font-size: 1.2rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		text-transform: none;
		
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}

	.hamburger{
		font-size: 1.2rem;
		display:none;
	}

	@media(max-width: 1100px){

		nav {
		display: flex;
		align-items: center;
		display: grid;
		grid-template-columns: .5fr 5fr;
	
	
	}

	ul{
		padding: 7rem 1rem;
		flex-direction: column;
	}

	li{
		height: auto;
	}
	
	
	.hamburger{
		display: block;
		z-index: 1001;
	}

	.links{
		position: absolute;
		top: 0;
		left: 0;
		height: 100vh;
		background-color: rgb(185 193 204);
		flex-direction: column;
		display: none;
		transform: translateX(-100%);
		transition: transform 0.3s ease;
		border-radius: 5px;
	
		z-index: 1000;
		}

		.links.active{
			display: flex;
			transform: translateX(0);
		}

	.middle{
		justify-content: center;

	}

	.middle.shifted{
		transform: translateX(0%);
	}
	.middle a{
		font-size: 2rem;
	}
	

	}

</style>
