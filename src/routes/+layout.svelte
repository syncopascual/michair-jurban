<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import NavBar from '$lib/components/NavBar.svelte';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="bg-surface min-h-screen">
	<header class="z-50 sticky inset-x-0 top-0">
		<NavBar />
	</header>
	{@render children()}
</div>
