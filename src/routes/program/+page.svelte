<script lang="ts">
	
import bilde from '$lib/images/bakgrunnsbilde.jpg';
</script>

<svelte:head>
	<title>Program</title>
	<meta name="description" content="About this app" />
</svelte:head>


 <section id="Program">
<div class="text-column">

	<h1> Program for dagen</h1>

</div>

<div class="heia">

	<div class="vb">
		<div class="vielsebilde"></div>
	</div>
	
	<div class="vielse">
		<h3>Vielse</h3>
		<br>
		<br>
		<h4> 25 juli 2026</h4>
		<br>
		<h4> Kl 14:00</h4>
		<br>
		<p> Sauråsbakken 20, 5131 Bergen, Norge</p>
	</div>
</div>


<div class="heia">

		<div class="vielse">
				<h3>Festen</h3>
				<br>
				<br>
				<h4> 25 juli 2026</h4>
				<br>
				<h4> Kl 15:30 - 01:00</h4>
				<br>
				<p> Olderkjerret 6, 5108 Hordvik, Norge</p>
			</div>
	<div class="vb">
		<div class="festbilde"></div>
	</div>

</div>


</section>

<style>

	h1 {
		text-align: left;
		
	}

	h3{
	font-size: 3rem;
	display: inline-block;
	}
	h4{
		font-size: 2rem;
		text-align: center;
	}

	p {
		text-align: left;
		font-size: 2rem;
		
		
	}

	.heia{
		display: flex;
		width: 100%;
		padding: 15px;
	}
	
	.vb{
		width: 50%;
		padding: 15px;
	}
	.vielsebilde{
		height: 100%;
		width: 100%;
		background-size: cover;
		background-position: center center;
		background-image: url("../../lib/images/bakgrunnsbilde.jpg");
		
	}

	.vielse{
		display: column;
		align-items: center;
		justify-content: center;
		padding-bottom: 15px;
		text-align: center;
	}

	.festbilde{
height: 100%;
		width: 100%;
		background-size: cover;
		background-position: center center;
		background-image: url("../../lib/images/bryllupsfest.jpg");
	}
</style>
