<script lang="ts">
	import Header from './Header.svelte';
	import './layout.css';

	let { children } = $props();
	 let open = $state();

	 let toggleMenu = () =>{
		open = !open;
	}
	let closeMenu =() =>{
		open = false;
	}
	

</script>

<div class="app" >
	<Header {open} {toggleMenu} {closeMenu} />
	<main class="app" class:shifted={open}>{@render children()}</main>


</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}
	.app {
  transition: transform 0.3s ease;
}
	.app.shifted {
  	transform: translateX(0%);
}

</style>
