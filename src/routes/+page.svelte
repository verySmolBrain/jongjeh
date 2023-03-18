<script>
    import Draggable from '../lib/Draggable.svelte';
    import RollingText from '../lib/RollingText.svelte';

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

<style>
    .body {
        background-image:url('folder/image.gif');
        background-size:100%;
        background-repeat: repeat-y;
        background-attachment: fixed;
        height:100%;
        width:100%;
    }
</style>

<h1> <RollingText /> </h1>

<h1> PLEASE ZOOM OUT IF YOU WANT A BETTER VIEW </h1>

<h1> RIGHT CLICK IMAGE (OPEN IMAGE IN NEW TAB) NOTE: NOT OPEN LINK IN NEW TAB </h1>

<h1> THE IMAGES ARE DRAGGABLE </h1>

<img src = "https://i0.wp.com/www.printmag.com/wp-content/uploads/2021/02/4cbe8d_f1ed2800a49649848102c68fc5a66e53mv2.gif?fit=476%2C280&ssl=1" class = "body"/>

<Draggable>
    <a href = "">
        <img src="/1.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555; alt: Image1;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/2.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555; alt: Image2;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/3.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555; alt: Image3;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/4.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555; alt: Image4;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/5.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555; alt: Image5;"  />
    </a>
</Draggable>
