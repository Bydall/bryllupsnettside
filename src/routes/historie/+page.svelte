<script lang="ts">
	

</script>

<svelte:head>
	<title>Vår Historie</title>
	<meta name="description" content="Vår Historie" />
</svelte:head>

<section id="Historie">
<div class="text-column">

	<h1> Vår historie</h1>

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

.heia{
	flex-wrap: wrap;

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

	.hotellrom{
		width: 50%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 15px;
		text-align: center;
	}

	.historiebilde{
		width: 100%;
		padding-top: 70%;
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
		.hotellrom{
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

		.hotellromtekst{
			align-items: center;
		}

	}

</style>