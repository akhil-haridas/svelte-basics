<script>
	const mobileCompanies = ["Apple","Pixel","Nothing","Samsung","OnePlus"]
</script>

<div>
	{#each mobileCompanies as comapny,index}
		<h1>{comapny}</h1>
	{/each}	
</div>