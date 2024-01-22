<script>
    const nameList = [
        {
            firstName :"Akhil",
            lastName : "K"
        },
        {
            firstName : "Sagar",
            lastName : "Samanta"
        },
    ]
</script>

<div>

    {#each nameList as name (name)}
        <slot firstName={name.firstName} lastName={name.lastName} />
    {/each}
    
</div>