<!-- <script>
    let cats = [
        {id:1, name:"masai"},
        {id:2, name:"svelte"}
        
    ]
</script>

<h1> the famous cats ofYoutub </h1>

<ul>
    {#each cats as {id,name},i}
    <li>
        {i+1}: name
    </li>
{/each}
</ul>

<style>
    li{
        color: red;
    }
</style> -->/



<script>
    import Things from "./Things.svelte";

    let things = [
        {id:1, color: 'darlblue'},
        {id:2, color:'red'},
        {id:3, color: 'gold'},
        {id:4,  color:'teal'},
        {id:5, color: 'black'},
        {id:6, color: 'deeppink'}
    ]

    const handleClick = () =>{
        things = things.slice(1);

    }
</script>

<button on:click={handleClick}> remove first things</button>

<div style="display: grid; grid-template-columns: 1fr 1fr; grid-gap: 1em">
    <div>
        <h2>keyed</h2>
        {#each things as thing (thing.id)}
        <Things current={thing.color}/>
        {/each}
    </div>

    <div>
        <h2>unkeyed</h2>
        {#each things as thing}
            <Things current={thing.color}/>
        {/each}
    </div>
</div>



