<script>
	import '$lib/styles/reset.css';
	import '$lib/styles/global.css';
	import Screen from '$lib/components/Screen.svelte';
</script>

<svelte:head>
	<meta name="theme-color" content="black" />
</svelte:head>

<Screen>
	<slot />
</Screen>
