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
</section>

<style>

h1{
	margin: 0;
	text-align: left;
}

a {
	
	text-align: center;
	font-size: 1.2rem;
	display: block;
	margin: 1rem;
	padding: .5rem 1rem;
	border: none;
    border-radius: 5px;
    cursor: pointer;
	width: 40%;

} 

.lists{
	
	display: flex;
	justify-content: center;
	flex-direction: row;
	margin: 1rem;
	width: 100%;

}


.vipps {

	background-color: rgb(255 91 36);
	color: rgb(255, 255, 255);

}

.christiania{
	background-color: rgb(255, 255, 255);
	color: rgb(0, 0, 0);
}

.kitchn {
	background-color: rgb(0, 0, 0);
	color: rgb(255, 255, 255);
}

.text-column{

	display:flex;
	flex-direction: column;
	padding: .3rem;
	width: 100%;
	

}

@media (max-width: 768px) {

	a {
	text-align: center;
	font-size: 1rem;
	display: flex;
	align-items: center;
	flex-direction: row;
	margin: 1rem;
	padding: 0 .4rem 0 .4rem;
	border: none;
    border-radius: 5px;
    cursor: pointer

	}
	


.lists{
	display: column;
	justify-content: center;
	flex-direction: row;
	margin: 1rem;
	width: 100%;

}

h1{
	justify-content: center;
}
	
	}


</style>