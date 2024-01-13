<script>
	// const mobileCompanies = ["Apple","Pixel","Nothing","Samsung","OnePlus"]
	const mobileCompanies = [{name:"Apple"},{name:"Pixel"},{name:"Nothing"},{name:"Samsung"},{name:"OnePlus"}]

</script>

<div>
	{#each mobileCompanies as company}
	<input type="text" placeholder="Enter name" />
		<h1>{company}</h1>
	{/each}	
</div>