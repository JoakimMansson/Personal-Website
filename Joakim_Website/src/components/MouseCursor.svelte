<script>
	import { spring } from 'svelte/motion';

	let coords1 = spring(
		{ x: 0, y: 0 },
		{
			stiffness: 0.2,
			damping: 0.3
		}
	);

	let coords2 = spring(
		{ x: 0, y: 0 },
		{
			stiffness: 0.1,
			damping: 0.3
		}
	);

	let size = spring(10);

</script>

<svelte:window
	on:mousemove={(e) => {
		coords1.set({ x: e.clientX, y: e.clientY })
		coords2.set({ x: e.clientX, y: e.clientY })
	}}
	on:mousedown={(e) => {
		size.set(30);
	}}
	on:mouseup={(e) => {
		size.set(10);
	}}
/>

<svg
	class ="w-full h-full"
>
	<circle cx={$coords1.x} cy={$coords1.y} r={$size} stroke="#FFF" stroke-width="1" fill-opacity="1"/>
	<circle cx={$coords2.x} cy={$coords2.y} r={$size/4} fill="#282828"/>
</svg>

<style>
	:global(body) {
		cursor: auto;
	}
	
	.w-full {
		width: 100%;
	}
	
	.h-full {
		height: 100%;
	}
	
	svg {
		position: fixed;
		top: 0;
		left: 0;
		pointer-events: none;
	}
</style>