<script>
    let m = {x:0, y:0};
</script>

<div on:mouseover={(e=> (m = {x: e.clientX, y: e.clientY}))}>
    the mouse postion is {m.x} x {m.y} y
</div>

<style>
    div{
        width: 100%;
        height: 100%;
        color: teal;
    }
</style>