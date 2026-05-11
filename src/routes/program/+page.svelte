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
	<div class="center">
		<h3>Vielse</h3>
		<br>
		<p> 25. juli 2026</p>
		<br>
		<h4> Kl 14:00</h4>
		<br>
		<p class="sted"> Sauråsbakken 20, 5131 Bergen, Norge</p>
		</div>
	</div>
</div>


<div class="heia">

		<div class="vielse">
			<div class="center">
				<h3>Festen</h3>
				<br>
				<p> 25. juli 2026</p>
				<br>
				<h4> Kl 15:30 - 01:00</h4>
				<br>
				<p class="sted"> Olderkjerret 6, 5108 Hordvik, Norge</p>
			</div>
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

	h3,h4, p {
		font-weight: 200;
		display: inline-block;
	}
	h1 {
		text-align: left;
		font-size: 30px;
		font-weight: bolder;
		
	}

	h3{
	font-size: 36px;
	padding: 5px 20px 5px 20px;
	margin: 0px;
	margin-bottom: 8px;
	}
	h4{
		font-size: 25.2px;
		text-align: center;
		padding: 5px 20px 5px 20px;
		margin: 0px;
		margin-top: 5px;
	}

	p {
		text-align: center;
		font-size: 22.5px;
		padding: 5px 20px 5px 20px;
		margin-top: 16px;
		margin-bottom: 0px;
		
		
	}
	.center{
		text-align: center;
	}
	.sted{
		font-size: 14.4px;
		margin-top: 4px;
	}

	.text-column{
		text-align: left;
		padding: 15px;
		font-weight: bolder;
	}
	
	.vielsebilde{
		width: 100%;
		padding-top: 70%;
		position: relative;
		background-size: cover;
		background-position: center 30%;
		background-image: url("../../lib/images/bakgrunnsbilde.jpg");
		
	}

	.vielse{
		width: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 15px;
		padding-bottom: 100px;
		
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

		h1{
			font-size: 17.1px;
		} 
		
		h4{
			font-size: 17.1px;
			margin-top: 0px;
		}

		 h3{
			font-size: 19.8px;
			margin-bottom: 0px;
		 } 
		 
		.sted{
			font-size: 12.6px;
			margin-top: 0px;
			margin-bottom: 5px;
		}
			p{
				font-size: 14.4px;
				margin-top: 0px;
		}

	}
</style>
