<script>
    import { onMount, onDestroy, beforeUpdate, afterUpdate  } from 'svelte'

    // onMount(()=>{
    //     console.log("Mounting....")
    //     return(()=>{
    //         console.log('Unmounting...')
    //     })
    // })

    // onDestroy(()=>{
    //     console.log("Component Destroyed")
    // })

    beforeUpdate(()=>{
        console.log('Before Update')
    })

    afterUpdate(()=>{
        console.log('After Update')
    })
</script>

<div>
<h1> Mount components</h1>
</div>