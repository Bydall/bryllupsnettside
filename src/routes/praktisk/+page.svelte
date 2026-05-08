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
			For dem som vil litt utenfor sentrum så er Clarion Hotell Edvard Grieg, på Sandsli, et veldig bra alternativ. </p>
	</div>
</div>
	

</div>
</section>

<style>


	h1{
		text-align: left;
	}
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
		background-position: center 30%;
		background-image: url("../../lib/images/hotellrom.jpg");
		

	}
	.hotellromtekst{
		text-align: left;
	}


	@media (max-width: 480px) {

	.text-column{

		display:block;
		padding: .3rem;
		width: 100%;
}
h1{
	padding: 0;
}

	}

</style>