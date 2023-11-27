<script>
	// @ts-ignore
	import Chase from '../components/chase.svelte';
</script>

<svelte:head>
	<title>Moxerit</title>
	<meta name="description" content="Chase's portfolio site" />
</svelte:head>

<article class="home-article">
		<div class="container">
			<a href="#" class="logo"><Chase/></a>
			<h1 class="name">Chase Alber</h1>
			<p class="slogan">Full-Stack Engineer | UI/UX Designer</p>
			<p class="location">Helena, Montana</p>
		</div>
		<div class="container-about">
			<h2>About me</h2>
			<p>From licking stamps to directing statewide projects, I enjoy a wide range of passions. <br> <br> Web accessibility is one of my most passionate - from Section 508 to AAA WCAG 2.2 standards. <br> <br> This site contains best practices I employ, inspirations, and my proudest works. <br> <br> I am currently available for consulting or employent oppurtunites. </p>
		</div>
</article>


<style>
	.home-article {
		display: flex;
		flex-direction: column;
		justify-content: start;
		align-items: center;
		margin-top: 10vh;
	}
	
	.container {
		align-self: center;
		text-align: center;
		min-height: 30vh;
		padding: 1rem;
		border-radius: 25px;
		margin-bottom: 5vh;
	}
	.container > h1 {
		margin: 0.2em;
	}
	.container > p {

		margin-top: 0.5em;
		
	}
	.container-about {
		box-shadow: 0px -3px 6px 0px var(--brown);
		background-color: var(--black);
		align-self: center;
		text-align: center;
		height: 60vh;
		padding: 1rem;
		margin-bottom: 2rem;
	}
	.container-about > h2 {
		margin: 0.5em;
		color: var(--light-parch);
	}
	.container-about > p {
		margin: 2em 0.2em;
		padding: 1em;
		color: var(--black);
		border-radius: 25px;
		background-color: var(--light-parch);
		box-shadow: 0px 4px 12px 2px var(--brown);
	}
	.name {
		font-size: 2.4rem;
		
	}
	.slogan {
		font-size: 1em;
		font-weight: 300;
	}

	@media (min-width: 905px) {
		.home-article {
			margin-top: 10vh;
		}
		.container-about {
			width: 30vw;
			background-color: var(--black);
			align-self: center;
			text-align: center;
			max-height: 30vh;
			padding: 1rem;
			border-radius: 50px;
			margin-bottom: 2rem;
		}
		.container-about > h2 {
		margin: 0.2em;
		color: var(--ivory);
		}
		.container-about > p {
			margin: 1em;
			padding: 1em;
			color: var(--black);
			border-radius: 25px;
			background-color: var(--light-parch);
		}
	}
</style>