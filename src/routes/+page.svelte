<script lang="ts">
	import Countdown from './Countdown.svelte'

	
</script>

<svelte:head>
	<title>Hjem</title>
	<meta name="description" content="Home Page" />
</svelte:head>

<section>

	<Countdown/>

</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.3;
		margin: 0;
	}


</style>
