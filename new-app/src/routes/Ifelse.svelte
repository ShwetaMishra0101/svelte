<script> 
    let user = {loggedIn : false};

    const handleToggle = () => {
        user.loggedIn = !user.loggedIn
    }
</script>


    {#if user.loggedIn}
    <button on:click={handleToggle}>log out</button>
    {:else} 
    <button on:click={handleToggle}>log in</button>
    {/if}
