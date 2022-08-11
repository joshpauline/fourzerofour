<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">

	import { onMount } from 'svelte';

	import Counter from '$lib/Counter.svelte';
	import init from 'wgpu_integration';

	onMount(async () => {
		init().then(() => console.log("WASM LOADED"));
	});

</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<canvas id="canvas_example" class="canvas-class"/>

<style>
	.canvas-class {
		width: 100vw;
		height: 100vh;
	}

</style>
