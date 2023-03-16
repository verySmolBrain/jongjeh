<script>
    import Draggable from './Draggable.svelte';

    let min_left = 0;
    let max_left = 150;

    let min_top = 0;
    let max_top = 50;

    function left() {
        return Math.random() * (max_left - min_left) + min_left;
    }

    function top() {
        return Math.random() * (max_top - min_top) + min_top;
    }
</script>

<Draggable>
    <a href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ">
        <img src="/1.png" style="position: absolute; left: {left()}vh; top: {top()}vh;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ">
        <img src="/2.png" style="position: absolute; left: {left()}vh; top: {top()}vh;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ">
        <img src="/3.png" style="position: absolute; left: {left()}vh; top: {top()}vh;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ">
        <img src="/4.png" style="position: absolute; left: {left()}vh; top: {top()}vh;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "https://www.youtube.com/watch?v=dQw4w9WgXcQ">
        <img src="/5.png" style="position: absolute; left: {left()}vh; top: {top()}vh;"  />
    </a>
</Draggable>