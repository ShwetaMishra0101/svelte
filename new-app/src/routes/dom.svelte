<script>
    let m = {x:0, y:0}

    function handleMouseMove(event) {
        m.x = event.clientX;
        m.y = event.clientY;
    }
</script>

<div on:mouseover={handleMouseMove}>
    the mouse postion is {m.x} x {m.y}  y
</div>