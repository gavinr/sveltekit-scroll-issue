<script>
	const links = [...Array(500).keys()];
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation. Sveltekit v next.272</p>

<ul>
	{#each links as link}
		<li><a sveltekit:prefetch href="links/{link}">{link}</a></li>
	{/each}
</ul>
