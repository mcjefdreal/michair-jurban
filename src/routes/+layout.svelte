<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import NavBar from '$lib/components/NavBar.svelte';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="p-5 bg-[#1da1f2]">
	<header class="z-50 sticky inset-x-0 p-3 top-3">
		<NavBar />
	</header>
	{@render children()}
</div>
