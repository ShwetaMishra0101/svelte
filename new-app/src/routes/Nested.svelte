<p>.... don't affect this element </p>

<script>
    let count = 0;
    const handleClick = () =>{
        count +=1;

    }
</script>

<button on:click={handleClick}>
    clicked {count} {count === 1 ? "time" : "times"}
</button>

<style>
    button{
        height: 10vh;
        width: 20vh;
        background-color: teal;
        color: wheat;
        border-radius: 10px;
    }
    button:hover{
        background-color: brown;
    }
</style>