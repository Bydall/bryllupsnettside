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
				<a href="#Program"  on:click={closeMenu}>Program</a>
			</li>
			<li aria-current={page.url.pathname === '/praktisk' ? 'page' : undefined}>
				<a href="#Praktisk" id="praktiskId" on:click={closeMenu}>Praktisk Info</a>
			</li>
			<li aria-current={page.url.pathname === '/historie' ? 'page' : undefined}>
				<a href="#Historie" id="historieId" on:click={closeMenu}>Vår Historie</a>
			</li>
			<li aria-current={page.url.pathname === '/onskeliste' ? 'page' : undefined}>
				<a href="#Onskeliste" id="onskId" on:click={closeMenu}>Ønskelister</a>
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
		font-family: 'Alex Brush';
		font-size: 36px;
		justify-content: center;

	}

	.links{
		display: block;
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
		font-weight: normal;
		font-size: 1rem;
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


	ul{
		padding: 200px 20px;
		margin:7px;
		margin-top: 15px;
		flex-direction: column;
	}

	li{
		height: auto;
		padding: 15px;
	}
	
	.hamburger{
		position: relative;
		z-index: 1002;
	}
	
	.hambtn{
		display: block;
		z-index: 1001;
		font-size: 28px;
	}

	nav {
		width: 100%;
	}

	nav a {
		font-size: 16px;
	}

	.links{
		position: absolute;
		top: 0;
		left: 0;
		height: 100vh;
		background-color: rgb(185, 193, 204);
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

	
	
	

	
	@media(min-width: 768px)and (max-width:992px){

		.middle a{
		font-size: 32px;
		}

		ul {
			padding-top: 180px;
		}

		li{
			padding: 12px;
		}

		.hambtn{
			font-size: 2.5rem;
		}

		
	}

	@media(min-width: 576px)and (max-width:767px){

		ul{
			padding:160px 16px;
		}
		
		li{
			padding: 9px;
		}

		.middle a {
			font-size: 32px;
		}

	}

	@media(max-width: 576px){

		nav{
			align-items: baseline;
		}

		ul{
				padding: 150px 16px;
			}

			li{
				padding: 9px;
			}
			
			
		.hambtn{
			align-items: center;
			font-size: 22px;
		}
		.links a {
			font-size: 12.8px;
		}

		.middle{
			position: relative;
			width: 100%;
			left:unset;
			transform: none;
		
		}

		.middle a{
			padding: 0px;
			text-align: left;
			font-size: 24px;
		}

}


</style>
