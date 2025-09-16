<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();

</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<h1 class="large">BRANCO VAN BEEK</h1>
<!-- <h1 class="large">{member.name}</h1> -->

{@render children?.()}