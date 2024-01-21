<script>
    import { onMount } from 'svelte'

    onMount(()=>{
        console.log("Mounting....")
        return(()=>{
            console.log('Unmounting...')
        })
    })
</script>

<div>
<h1> Mount components</h1>
</div>