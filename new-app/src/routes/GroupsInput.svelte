<script>
    let scoops =1;
    let flavours = ['min choc chip'];

    let menu = ['cookies and cream','min choc chip', 'ripple'];

function join(flavours){
    if(flavours.length===1) return flavours[0];
    return  `${flavours.slice(0,-1).join(',')} and ${flavours[flavours.length -1]}`
}
</script>

<h2>Size</h2>

<label for="">
    <input type="radio" bind:group={scoops} value={1}>
    One scoop
</label>

<label for="">
    <input type="radio" bind:group={scoops} value={2}>
    two scoop
</label>

<label for="">
    <input type="radio" bind:group={scoops} value={3}>
    Three scoop
</label>

<h2>flavours</h2>

{#each menu as flavour}

<label for="">
    <input type="checkbox" bind:group={flavours} value={flavour}>
    {flavour}
</label>
    
{/each}

{#if flavours.length === 0}
<p>please select at least one flavours</p>
{:else if flavours.length > scoops}
<p>con't order more flavours than scoops!</p>
{:else}
<p>
    you ordered {scoops}
    {scoops===1? 'scoop':'scoops'}
    of {join(flavours)}
</p>
{/if}

