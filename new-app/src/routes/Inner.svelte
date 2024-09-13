<script>
    import { createEventDispatcher } from "svelte";

    const dispatch = createEventDispatcher();

    const sayHello = () => {
        dispatch('message',{
            text:'hello'
        })

    }
</script>

<button on:click={sayHello}>click to say hello</button>