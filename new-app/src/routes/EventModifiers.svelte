<script>
    const handleClick =()=>{
        alert('no more alerts')
    }
</script>

<button on:click|once={handleClick}>click me</button>