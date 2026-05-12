<script lang="ts">
	
	let now = Date.now();
	let endDate = Date.UTC(2026,6,25,14,0);

	let days, hours, minutes, seconds;

	function updateTimer(){
		now = Date.now();

	let count = Math.round((endDate - now)/ 1000);

	days = Math.floor(count / 86400);
	hours = Math.floor((count % 86400 / 3600)) 
	minutes = Math.floor((count % 3600) / 60);
	seconds = count % 60;
	
	}
	
	setInterval(updateTimer,1000);
	
</script>

	<h1>{days} dager, {hours} timer, {minutes} minutter og {seconds} sekunder igjen  </h1>
	
<style>	
	h1 {
		width: 100%;
		font-family: 'Alex Brush';
		font-size: 32px;
		font-variant-numeric: tabular-nums;
	}

	@media(min-width: 768px) and (max-width:992px){
		h1{
			font-size: 28px;
		}
		
	}
	@media(min-width: 576px) and (max-width:768px){
		h1{
			font-size: 28px;
		}
	}

	@media(max-width:576px){
		h1{
			font-size: 14px;
		}
	}


</style>