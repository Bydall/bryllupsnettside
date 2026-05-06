<script lang="ts">

</script>

<svelte:head>
	<title>Ønskeliste</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">

	<h1>Ønskelister</h1>
	

	<div class="lists">
	<a class="onsk" href="https://onskeskyen.no/nb/wishlists/Rfu9e9tOmgLqW1Dc?sharedBy=EunZl6BQE0TgmFJE&utm_source=shortlink&utm_id=ep3xhn"> Ønskeskyen </a>
	<a class="christiania" href="https://www.cg.no/apps/giftregistry/registry/414094?_r=1&utm_source=gift_reggie&utm_medium=gift_reggie&utm_campaign=gift_reggie&utm_content=414094"> Christiania Glassmagasin </a>
	<a class="kitchn" href="https://www.kitchn.no/onskeliste/241866/"> Kitchn </a>

	</div>

</div>


<style>

h1{
	margin: 0;
}

a {
	
	text-align: center;
	font-size: 1.2rem;
	display: block;
	margin: 1rem;
	padding: .5rem 1rem;
	border: none;
    border-radius: 5px;
    cursor: pointer

} 

.onsk {

	background-color: rgb(5, 154, 190);
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

	a{
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
	display: flex;
	justify-content: center;
	flex-direction: row;
	margin: 1rem;
}

h1{
	justify-content: center;
}
	
	}


</style>