<script>
	import favicon from '$lib/assets/favicon.svg';

	let { member, children } = $props();
	
	import '../app.css';
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}
