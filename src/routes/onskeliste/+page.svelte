<script lang="ts">

</script>

<svelte:head>
	<title>Ønskeliste</title>
	<meta name="description" content="About this app" />
</svelte:head>

<section id="Onskeliste">
<div class="text-column">

	<h1>Ønskelister</h1>
	
	<div class="lists">
	<a class="vipps" href="https://qr.vipps.no/wish-list/940b0303-2db4-478d-f92b-08deaa80665d" target="_blank" rel="noopener noreferrer"> Vipps </a>
	<a class="christiania" href="https://www.cg.no/apps/giftregistry/registry/414094?_r=1&utm_source=gift_reggie&utm_medium=gift_reggie&utm_campaign=gift_reggie&utm_content=414094" target="_blank" rel="noopener noreferrer"> Christiania Glassmagasin </a>
	<a class="kitchn" href="https://www.kitchn.no/onskeliste/241866/" target="_blank" rel="noopener noreferrer"> Kitchn </a>

	</div>

</div>


<div class="gavetekst">

	<p> Hvis du vil gi en pengegave, så kan det gjøres til kontonummer: <br> 3000 90 05915 (Merk med navn)</p>

	</div>

</section>

<style>

#Onskeliste{
		max-width: 100%;
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		background-image: url("../../lib/images/footer_image.jpg");
		background-size: cover;
		background-position:center 70%;
		padding: 15px;
}

h1{
	text-align: center;
	width: 25%;
}

p{
	text-align: center;
	margin: 0 auto;
	color: rgb(255,255,255);
	font-size: 24px;
	
}

a {
	
	text-align: center;
	font-size: 1.2rem;
	display: block;
	margin: 2rem;
	padding: 1rem 1rem;
	border: none;
    border-radius: 5px;
    cursor: pointer;
	width: 20%;
	height: 100%;

} 

.lists{
	
	display: flex;
	justify-content: center;
	flex-direction: column;
	margin: 1rem;
	width: 100%;

}


.vipps{

	background-color: rgb(255 91 36);
	color: rgb(255, 255, 255);

}

.christiania{
	background-color: rgb(255, 255, 255);
	color: rgb(0, 0, 0);
	border: .2px solid black;

}

.kitchn {
	background-color: rgb(0, 0, 0);
	color: rgb(255, 255, 255);
}

.text-column{

	display:flex;
	flex-direction: column;
	margin: 0px auto;
	padding-top: 100px;
	padding-left: 15px;
	width: 100%;
	

}

.gavetekst{
	background-color: rgba(0, 0, 0, 0.5);
	width: 100vw;
	height: 25%;
	
	position: absolute;
	bottom:0;
	left:0;
	display: flex;
	align-items: center;
	
	}

 @media (min-width: 768px) and (max-width: 992px) {

	
	.text-column{
		padding-top: 120px;
		margin-bottom: 140px;
	}
	
	a{
		margin:20px;
		padding: 20px;
		width: 20%;
		font-size: 16.2px;
		text-align: center;
	}


	p{
		font-size: 16.2px;
	}

 }

  @media (min-width: 576px) and (max-width: 768px) {

	
	.text-column{
		padding-top: 120px;
		margin-bottom: 240px;
	}
	
	a{
		margin:20px;
		padding: 20px;
		width: 25%;
		font-size: 16.2px;
		text-align: center;
	}


	p{
		font-size: 16.2px;
	}

 }


	@media (max-width: 576px) {
		
		.lists{
			margin:0px;
			margin-top: 70px;
			align-items: center;
			flex-direction: row;
			

		}
		a{
			flex: 1;
			padding: 20px;
			margin: 10px;
			border: none;
    		border-radius: 5px;
    		cursor: pointer;
			width: 100%;
			font-size: 12.8px;

		}

		.text-column{
			padding: 15px;
			margin-top: 140px;
			margin-bottom: 270px;
		}

		.christiania{
			padding:10.98px;
		}

		.gavetekst{
			margin-top: 20px;
		}
		h1{
			align-items: left;
		}
		p{
				
			font-size: 12.8px;
			text-align: center;
		}
	}



</style>