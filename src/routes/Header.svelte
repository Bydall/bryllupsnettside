<script lang="ts">
	import { resolve } from '$app/paths';
	import { page } from '$app/state';

	export let open: boolean;
	export let toggleMenu: () => void;
	export let closeMenu: () => void;

</script>

<header>

	<div class="something">
	
	<nav>

	<div class="hamnav">
	<div class="hamburger">
		<button class="hambtn" on:click={toggleMenu}>
			{#if open}
			✕
			{:else}
			☰
			{/if}
		</button>
	</div>


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
	
	</div>
		
	<div class:shifted={open} class="middle">
		<a href={resolve('/')}>
		Mathilde og Håvard
		</a>
	</div>

	</nav>
</div>
	
</header>

<style>

.something{
	margin:	0 auto;
}
	header {
		
		padding: 1rem;
		display: block;
		
		
	}
	.hamnav{
		align-items: center;
	}

	.middle{
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
	}

	.middle a {
		font-family: 'Waterfall';
		font-weight:normal;
    	font-size: 2.2rem;
    	text-decoration: none;
		text-transform: none;
		text-align: left;
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
		margin: 0 auto;
		padding: 15px;
		width: 100%;
	
	
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
		color: rgb(0,51,25);
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

	.hambtn{
		font-size: 1.2rem;
		display:none;
	}

	@media(max-width: 1300px){

	ul{
		padding: 7rem 1rem;
		flex-direction: column;
	}

	li{
		height: auto;
	}
	
	.hamburger{
		position: relative;
		z-index: 1002;
	}
	
	.hambtn{
		display: block;
		z-index: 1001;
	}

	nav {
		width: 100%;
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
		width: 75%;
		position: absolute;
		left: 50%;
		transform: translateX(-50%);

	} 
	.middle.shifted{
		transform: translateX(-50%);
	}

	
	.middle a{
		font-size: 2rem;
		justify-content: center;
	}
	

	}
	@media(min-width: 768px)and (max-width:1300px){

		.middle a{
		font-size: 3rem;
		}

		ul {
			padding-top: 8rem;
		}

		li{
			padding: .2rem;
		}

		.hambtn{
			font-size: 2.5rem;
		}

		
	}
	@media(max-width: 400px){

		.hambtn{
			font-size: 1.2rem;
		}
		ul{
			padding: 6rem 1rem;
		}
		nav a{
			font-size: 1rem;
		}

	}


	@media(max-width: 320px){

		ul{
			padding: 5.2rem 1rem;
		}

		li{
			padding: .1rem;
		}
		.middle a {
			font-size: 1.7rem;
	}

	.hambtn{
		font-size: .7rem;
	}
	.links a {
		font-size: .7rem;
	}
}


</style>
