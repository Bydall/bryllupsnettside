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
	text-align: left;
	padding-left: 2.5rem;
	width: 20%;
}

p{
	text-align: center;
	margin: 0 auto;
	color: rgb(255,255,255);
	font-size: 24px;
	
}

a {
	display: flex;
	align-items: center;
	justify-content: center;
	font-size: 1.2rem;
	text-align: center;
	margin: 1.5rem;
	padding: 1rem 1rem;
	border: none;
    border-radius: 5px;
    cursor: pointer;
	width: 25%;
	box-sizing: border-box;
	height: 50px;
} 

.lists{
	
	display: flex;
	justify-content: center;
	flex-direction: column;
	margin: 1rem;
	margin-top: 6rem;
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
	padding-top: 5%;
	padding-left: 15px;
	width: 100%;
	

}

.gavetekst{
	background-color: rgba(0, 0, 0, 0.5);
	width: 100%;
	height: 25%;
	position: absolute;
	bottom:0;
	left:0;
	display: flex;
	align-items: center;
	
	}

 @media (min-width: 768px) and (max-width: 992px) {

	
	.text-column{
		padding-top: 10%;
		margin-bottom: 140px;
	}
	
	a{
		margin:20px;
		padding: 20px;
		width: 30%;
		font-size: 16.2px;
		text-align: center;
	}

	h1{
		padding-left: 35px;
	}

	.lists{
		margin-top: 3rem;

	}
	p{
		font-size: 16.2px;
	}

 }

  @media (min-width: 576px) and (max-width: 768px) {

	
	.text-column{
		padding-top: 9%;
	}

	.lists{
		margin-top: 8%;
	}
	
	a{
		margin:10px;
		padding: 20px;
		width: 32%;
		height:20px;
		font-size: 16.2px;
		text-align: center;
	}

	h1{
		padding-left: 4%;
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
			padding: 20px;
			margin: 10px;
			border: none;
    		border-radius: 5px;
    		cursor: pointer;
			width: 33%;
			font-size: 11px;

		}

		.text-column{
			padding: 15px;
			margin-top: 10svh;
		}


		.gavetekst{
			margin-top: 20px;
		}
		h1{
		padding-left: 0.1%
	}

		p{
				
			font-size: 11px;
			text-align: center;
		}
	}

	@media (max-height: 500px) and (orientation: landscape){

		.text-column{
			padding-top:2svh;
		}
		
		.lists{
			margin-top: 1%;
		}
	}



</style>