<script>
    const nameList = [
        {
            firstName :"Akhil",
            lastName : "k"
        },
        {
            firstName : "Sagar",
            lastName : "Samanta"
        }
    ]
</script>

<div>

    {#each nameList as name (name)}
        <h1>{name.firstName} : {name.lastName}</h1>
    {/each}
    
</div>