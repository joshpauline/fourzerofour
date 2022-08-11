<script lang="ts">
	import { page } from '$app/stores';
	import logo from './404.png';
</script>

<header>
	<div class="corner">
		<a href="https://kit.svelte.dev">
			<img src={logo} alt="SvelteKit" />
		</a>
	</div>

	<div class="corner">
		<!-- TODO put something else here? github link? -->
	</div>

</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
	}

	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		padding: 1em;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 3em;
		height: 3em;
		object-fit: contain;
	}

	a:hover {
		color: var(--accent-color);
	}
</style>
