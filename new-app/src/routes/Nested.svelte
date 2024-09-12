<!-- <p>.... don't affect this element </p>

<script>
    let count = 0;

// $ means re-run whenever these value chjange

$: doubled = count * 2;
$: duadr = count * 2;

$: if(count >= 10){
    alert(`count is  dangerously high !`)
    count = 9

}

    const handleClick = () =>{
        count +=1;

    }
</script>

<button on:click={handleClick}>
    clicked {count} {count === 1 ? "time" : "times"}
</button>
<p>{count} * 2  =  {doubled}</p>
<p>{count} * 2  =  {duadr}</p>

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
</style> -->


<script>
    export let answer =  '100';
</script>

<p>This is answer is  {answer}</p>




