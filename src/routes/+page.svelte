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

<h1> JONGJEH </h1>

<h1> PLEASE ZOOM OUT IF YOU WANT A BETTER VIEW </h1>

<h1> RIGHT CLICK OPEN IMAGE IN NEW TAB </h1>

<p1> I've become so much like Eren Jaeger, it's scary.

    I wear black cardigans, verbally assault women, and physically assault my friends. When I look in the mirror, I can't help but say "戦い, 戦い" (which means fight, fight in american.) I grew my hair out long because I don't care so now I have to wear it in a bun and I don't care what people think so shut fuck up Hange! I always leave an open wound on my hand, and go out of my way to show it to everyone so they are reminded that I am in control. When I see dogs being taken on walks I get mad at them for not being free like I am. I can't have sex with my girlfriend anymore without forcing her to dress up as Mikasa or Historia, both of whom remind me of Armin. When I order fast food, I refuse to call them french fries and insist on calling them freedom fries. I just keep moving forward, until my enemies are destroyed.</p1>

<Draggable>
    <a href = "">
        <img src="/1.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/2.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/3.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/4.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555;"  />
    </a>
</Draggable>

<Draggable>
    <a href = "">
        <img src="/5.png" style="position: absolute; left: {left()}vh; top: {top()}vh; border: 5px solid #555;"  />
    </a>
</Draggable>