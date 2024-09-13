<script>
    let name ='';
    let a =1;
    let b=2;

    // /for check input
    let yes = false

</script>

<input bind:value={name} placeholder="Enter your name">
<p>hello {name||'stranger'}</p>


<!-- numeric inputs -->

<label for="">
    <input type="number" bind:value={a} min="0" max="20">
    <input type="range" bind:value={a} min="0" max="20">

</label>

<label for="">
    <input type="number" bind:value={b} min="0" max="20">
    <input type="range" bind:value={b} min="0" max="20">
    
</label>

<p> {a} + {b} = { a + b  } </p>


<!-- check input -->

<label for="">
    <input type="checkbox" bind:checked={yes} name="" id="">
    yes send me regular email spam
</label>

{#if yes}
<p>thank you . we will bombard your inbox and sell your personal details.</p>
{:else}
<p>you most opt-in to continue . if you'er the product.</p>

{/if}

<button disabled={!yes }> subscribe </button>

