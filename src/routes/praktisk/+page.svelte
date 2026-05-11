<script lang="ts">
	

</script>

<svelte:head>
	<title>Praktisk Info</title>
	<meta name="description" content="Praktisk Info" />
</svelte:head>

<section id="Praktisk">
<div class="text-column">

	<h1> Praktisk info</h1>

<div class="heia">

	<div class="vb">
		<div class="hotellrombilde"></div>
	</div>
	
	<div class="hotellrom">
		<h3>Reise og overnatting</h3>
		<br>
		<p class="hotellromtekst"> Det er mulighet for overnatting på hotellene i Bergen sentrum. 
			<br>
			For dem som vil bo litt utenfor sentrum, så er Quality Hotel Edvard Grieg et veldig bra alternativ. </p>
	</div>
</div>

<div class="heia">

	
	<div class="transport">
		<h3>Transport</h3>
		<br>
		<p class="transporttekst"> Det tar  ca. 15 min å kjøre fra Åsane Gamle Kirke til Hordvik Bedehus. 
							       Det er stor parkeringsplass på baksiden av bygget.  
		</p>
	</div>

	<div class="vb">
		<div class="transportbilde"></div>
	</div>
</div>
	

</div>
</section>

<style>



	p{
		text-align: left;
		line-height: 2rem;
		padding: 0;
	}

	#Praktisk{
		padding: 15px;
		position: relative;
		max-width: 1100px;
		box-sizing: border-box;
		margin: 0px auto;
	}

	h1 {
		text-align: left;
		
	}

	h3{
	font-size: 36px;
	display: inline-block;
	padding-right: 50px;
	}

	p {
		text-align: center;
		font-size: 18px;
		
		
	}

	.hotellrom{
		width: 50%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 15px;
		text-align: center;
	}

	.hotellrombilde{
		width: 100%;
		padding-top: 70%;
		position: relative;
		background-size: cover;
		background-position: center;
		background-image: url("../../lib/images/hotellrom.jpg");

	}
	.hotellromtekst{
		text-align: left;
	}

	.transport{
		width: 50%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding: 15px;
		text-align: center;
	}

	.transport{
		
		padding:15px;
	}
	.transporttekst{
		text-align: left;
	}

	.transportbilde{
		width: 100%;
		padding-top: 70%;
		position: relative;
		background-size: cover;
		background-position: center;
		background-image: url("../../lib/images/Hordvik_Bedehus.webp");

	}

	@media(min-width:768px) and (max-width:992px){
		h3{
			font-size: 28.8px;
		}
		p{
			font-size: 16.2px;
		}
	}

	@media(max-width: 576px){
		.heia {
			flex-wrap: wrap;
		}
		.vb{
			order: -1;
			width: 100%;
		}
		.hotellrom, .transport{
			padding-bottom: 0px;
			width: 100%;
		}
		h1{
			font-size: 19.8px;
		}

		 h3{
			font-size: 17.2px;
			padding: 0;
		}
			p{
				font-size: 12.8px;
				line-height: 24px;
		}

		.hotellromtekst,.transporttekst{
			align-items: center;
		}

	}

</style>