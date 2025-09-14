<script lang="ts">
	import favicon from '$lib/assets/favicon.png';
	import logo from '$lib/assets/logo.svg';
	import '@awenovations/aura/dist/tokens/_variables.css';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}

<style lang="scss">
  	@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

  :global(html, body) {
		background: var(--aura-background);
		font: var(--aura-default-regular);
		color: var(--aura-font-color);
		height: 100%;
	}

</style>
