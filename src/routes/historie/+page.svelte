<script lang="ts">
	

</script>

<svelte:head>
	<title>Vår Historie</title>
	<meta name="description" content="Vår Historie" />
</svelte:head>

<section id="Historie">
<div class="text-column">

	<h1> Vår Historie</h1>

<div class="heia">

	<div class="vb">
		<div class="historiebilde"></div>
	</div>
	
	<div class="historie">
		<p class="hotellromtekst"> 
			Vi møttes for første gang på julebordet til 'Unge Voksne' i Betlehem desember 2024.
			Håvard spurte Mathilde om hun hadde noen anbefalinger blant kakene, og hun svarte: "Sjokoladekaken kan anbefales."
			Fire måneder senere spurte Håvard Mathilde ut på date - resten er historie.
			<br>
			21. august 2025 fridde Håvard til Mathilde og spurte om hun ville gifte seg med han. Mathilde svarte: "JA!"

		</p>
	</div>
</div>
	

</div>
</section>

<style>

#Historie{
	display: flex;
	align-items: center;
}
.text-column{
	display: flex;
	align-items: center;
	margin-top: 100px;
	margin-bottom: 100px;
}


.vb{
	width: 100%;
}

	p{
		text-align: left;
		line-height: 34px;
		padding: 0;
	}

	#Historie{
		padding: 15px;
		position: relative;
		max-width: 1100px;
		box-sizing: border-box;
		margin: 0px auto;
		align-items: center;
		height:100vh;
	}

	h1 {
		padding: 15px;
		text-align: left;
		
	}

	p {
		margin-top: 10px;
		text-align: center;
		font-size: 18px;
		line-height: 34px;
		margin-bottom: 8px;
		padding: 15px;
		
		
	}
	.historie{
		width: 100%;
	}


	.historiebilde{
		width: 100%;
		padding-top: 100%;
		position: relative;
		background-size: cover;
		background-position: center 25%;
		background-image: url("../../lib/images/historie_bilde.jpg");
		filter: grayscale(100%);
		

	}
	.hotellromtekst{
		text-align: left;
	}

	@media(min-width:768px) and (max-width:992px){
		
		.vb{
			display: flex;
			padding: 0px;
		}
		
		p{
			font-size: 16.2px;
		}
	}

	@media(min-width:576px) and (max-width:768px){

		.heia{
			display: flex;
			width: 100%;
			align-items: center;
		}

		.vb{
			display: flex;
			padding:0px;
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

		h1{
			font-size: 19.8px;
		}

			p{
				font-size: 12.8px;
				line-height: 24px;
		}

		.hotellromtekst{
			align-items: center;
		}

	}

</style>