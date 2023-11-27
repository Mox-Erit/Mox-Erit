<script>
		import PostCard from '../../components/post-card.svelte';
		export let data;
</script>

<svelte:head>
    <title>Portfolio</title>
    <meta name="description" content="Projects I have created and designed from software to 3D models" />
</svelte:head>



<h1>Projects</h1>
<div class="portfolio-items-wrap">
	{#each data.posts as post}
		<a href='portfolio/{post.slug}' class="portfolio-item">
			<PostCard {...post}/>
		</a>
	{/each}
</div>



<style>
	h1 {
		margin-bottom: 1rem;
		color: var(--black);
	}
	.portfolio-items-wrap {
		padding: 1.5rem;
		display: flex;
		flex-direction: column;
		margin-top: 10vh;
		overflow-y: scroll;
	}
	.portfolio-item:hover {
		transition: all 0.2s ease-in-out;
		box-shadow: 0em 0.5em 1em 0 var(--brown);
	}
	.portfolio-item {
		border-radius: 50px;
		display: flex;
		width: 100%;
		background: var(--parchment);
		margin-bottom: 2rem;
		min-height: 15vh;
		box-shadow: 0em 0.2em 0.7em 0 var(--brown);
	}
	@media (min-width: 905px) {
	.portfolio-items-wrap {
		gap: 3rem;
		padding: 1.5rem;
		display: flex;
		flex-wrap: wrap;
		flex-direction: row;
		margin-top: 10vh;
		overflow-y:unset;
	}
	.portfolio-items-wrap > a {
		flex: 40%;
	}
	.portfolio-item {
		border-radius: 50px;
		display: flex;
		width: 100%;
		background: var(--parchment);
		margin-bottom: 1rem;
		min-height: 15vh;
		box-shadow: 0em 0.2em 0.7em 0 var(--brown);
	}
	
	}
</style>