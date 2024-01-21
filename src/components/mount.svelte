<script>
    import { onMount, onDestroy  } from 'svelte'

    // onMount(()=>{
    //     console.log("Mounting....")
    //     return(()=>{
    //         console.log('Unmounting...')
    //     })
    // })

    onDestroy(()=>{
        console.log("Component Destroyed")
    })
</script>

<div>
<h1> Mount components</h1>
</div>