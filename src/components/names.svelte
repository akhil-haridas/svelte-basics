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
        {
            firstName : "Sagar",
            lastName : "Mali"
        },
        {
            firstName: 'Rahul', 
            lastName: 'Sharma'
        },
        {
            firstName:"John",  
            lastName:"Doe"
        }
    ]
</script>

<div>

    {#each nameList as name (name)}
        <slot firstName={name.firstName} lastName={name.lastName} />
    {/each}
    
</div>