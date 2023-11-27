<script>
		import PostCard from '../../components/post-card.svelte';
		import { fade } from 'svelte/transition';
		export let data;
</script>

<svelte:head>
    <title>Portfolio</title>
    <meta name="description" content="Projects I have created and designed from software to 3D models" />
</svelte:head>



<h1 in:fade>Projects</h1>
<div class="portfolio-items-wrap" in:fade>

	{#each data.posts as post}
		<a href='portfolio/{post.slug}' class="portfolio-item">
			<PostCard {...post}/>
		</a>
	{/each}
</div>



<style>
	h1 {
		margin: 2rem 2rem 0rem 2rem;
		margin-top: 10vh;
		font-family: 'Goth-Med';
		color: var(--brown);
		opacity: 90%;
	}
	.portfolio-items-wrap {
		padding: 1.5rem;
		display: flex;
		flex-direction: column;
		height: 100%;
		margin: auto;
		width: 100%;
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
		margin-bottom: 4rem;
		min-height: 42vh;
		box-shadow: 0em 0.2em 0.7em 0 var(--brown);
	}
	@media (min-width: 905px) {
	.portfolio-items-wrap {
		padding: 1.5rem;
		display: flex;
		flex-wrap: wrap;
		flex-direction: row;
		margin-top: 10vh;
	}
	.portfolio-items-wrap > a {
		flex: 30%;
		margin: 3em;
	}
	.portfolio-item {
		border-radius: 50px;
		display: flex;
		
		background: var(--parchment);
		margin-bottom: 1rem;
		min-height: 15vh;
		box-shadow: 0em 0.2em 0.7em 0 var(--brown);
	}
	
	}
</style>