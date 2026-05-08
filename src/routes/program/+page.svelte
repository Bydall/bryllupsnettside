<script lang="ts">
	
import bilde from '$lib/images/bakgrunnsbilde.jpg';
</script>

<svelte:head>
	<title>Program</title>
	<meta name="description" content="About this app" />
</svelte:head>


 <section id="Program">

<div class="program">	
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



</div>


</section>

<style>

	.program{
		margin: 0px auto;
		display: block;
	}

	h1, h3,h4, p {
		color: rgb(0,51,25)
	}
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
		text-align: center;
		font-size: 2rem;
		
		
	}

	.text-column{
		text-align: left;
		padding: 15px;
	}
	
	.vielsebilde{
		width: 100%;
		padding-top: 70%;
		position: relative;
		background-size: cover;
		background-position: center 30%;
		background-image: url("../../lib/images/bakgrunnsbilde.jpg");
		
	}

	.vielse, .hotellrom{
		width: 50%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 15px;
		text-align: center;
	}

	.festbilde{
		padding-top: 70%;
		background-size: cover;
		background-position: center center;
		background-image: url("../../lib/images/bryllupsfest.jpg");
	}


	@media(max-width: 576px){
		.heia {
			flex-wrap: wrap;
		}
		.vb{
			order: -1;
			width: 100%;
		}
		.vielse{
			padding-bottom: 0px;
			width: 100%;
		}

		h1, h3, h4{
			font-size: 1.7rem;
		}
			p{
				font-size:1.5rem
		}

	}
</style>
