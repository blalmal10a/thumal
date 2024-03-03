<script>
	import { interpolateLab } from 'd3-interpolate';
	import { tweened } from 'svelte/motion';

	const colors = ['rgb(12, 211, 233)', 'rgb(64, 225, 201)', 'rgb(3, 103, 208)'];

	const color = tweened(colors[0], {
		duration: 800,
		interpolate: interpolateLab
	});
</script>

{#each colors as c}
	<button style="background-color: {c}; color: white; border: none;" on:click={(e) => color.set(c)}>
		{c}
	</button>
{/each}

<h1 style="color: {$color}">{$color}</h1>