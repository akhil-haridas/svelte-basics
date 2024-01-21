<script>
  import { onMount } from "svelte";


    let todos = []

    const fetchtodos = async ()=> {
        const response = await fetch('https://jsonplaceholder.typicode.com/todos')
        todos = await response.json()
    }
    onMount(()=>{
        fetchtodos()
    })

</script>

<main class="todo-list-wrapper">
    <h1>TODO LIST </h1>
    <div class="todo-wrapper">
        <span>✅</span>
        <h3>Todo item</h3>
    </div>
</main>

<style>
    .todo-list-wrapper {
        background-color: black;
        height: 100vh;
        display: flex;
        flex-direction: column;
        place-items: center;
    }

    .todo-wrapper {
        display: flex;
        place-items: center;
        width: 100%;
        background-color: darkgray;
    }
</style>