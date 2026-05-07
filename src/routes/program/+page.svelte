<script lang="ts">
	

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
		<div class="vielsebilde">
		</div>
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
	}
	
	.vb{
		width: 50%;
		padding: 15px;
	}
	.vielsebilde{
		background-image: url("../../lib/images/bakgrunnsbilde.jpg");
		background-size: cover;
		background-position: center center;
		
	}

	.vielse{
		display: column;
		align-items: center;
		justify-content: center;
		padding-bottom: 15px;
		text-align: center;
	}
</style>
