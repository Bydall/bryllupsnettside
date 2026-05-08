<script lang="ts">
	import Countdown from './Countdown.svelte'

	
</script>

<svelte:head>
	<title>Hjem</title>
	<meta name="description" content="Home Page" />
</svelte:head>

	<div class="countdown">
	<Countdown/>
</div>
<style>
	.countdown {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.3;
		margin: 0;
		
	}

	


</style>
