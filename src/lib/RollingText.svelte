<script>
	import { onMount, onDestroy } from 'svelte';
	import { slide } from 'svelte/transition';
	
	let greetings = ['JONGJEH', 'GIZTURD'];
	let index = 0;
	/**
     * @type {number | undefined}
     */
	let roller;
	
	onMount(() => {
		roller = setInterval(() => {
			if (index === greetings.length - 1) index = 0;
			else index++;
		}, 1250);
	});
	
	onDestroy(() => {
		clearInterval(roller);
	});
</script>

{#key index}
	<h1 transition:slide>{greetings[index]}!</h1>
{/key}