<script>
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
</style>