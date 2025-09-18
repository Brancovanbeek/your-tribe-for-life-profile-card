<script>
	import favicon from '/assets/favicon.svg';

	let { member, children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}
