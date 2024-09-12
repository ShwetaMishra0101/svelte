<!-- <script> 
    let user = {loggedIn : false};

    const handleToggle = () => {
        user.loggedIn = !user.loggedIn
    }
</script>


    {#if user.loggedIn}
    <button on:click={handleToggle}>log out</button>
    {:else} 
    <button on:click={handleToggle}>log in</button>
    {/if} -->


    <script>
        let x=7;
        </script>
        
        {#if x>10}
          <p>hii</p>
          {:else if 5>x}
          <p>is less </p>
          {:else}
          <p>{x}  in between </p>
        {/if}
