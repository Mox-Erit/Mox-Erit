<script>
		import PostCard from '../../components/post-card.svelte';
		export let data;
</script>

<svelte:head>
    <title>Portfolio</title>
    <meta name="description" content="Projects I have created and designed from software to 3D models" />
</svelte:head>




<div class="portfolio-items-wrap">
	{#each data.posts as post}
		<a href='portfolio/{post.slug}' class="portfolio-item">
			<PostCard {...post}/>
		</a>
	{/each}
</div>



<style>
	.portfolio-items-wrap {
		padding: 1.5rem;
		display: flex;
		flex-direction: column;
	}
	.portfolio-item:hover {
		transition: all 0.2s ease-in-out;
		box-shadow: 0em 0.5em 1em 0 var(--brown);
	}
	.portfolio-item {
		display: flex;
		flex-grow: 1;
		background: var(--parchment);
		margin-bottom: 1rem;
		min-height: 18%;
		box-shadow: 0em 0.2em 0.7em 0 var(--brown);
	}
</style>