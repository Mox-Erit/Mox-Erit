<script>
	// @ts-ignore
	import Chase from '../components/chase.svelte';
	import { fade } from 'svelte/transition';
</script>

<svelte:head>
	<title>Moxerit</title>
	<meta name="description" content="Chase's portfolio site" />
</svelte:head>

<article class="home-article" in:fade>
		<div class="container">
			<a href="#" class="logo"><Chase/></a>
			<h1 class="name">Chase Alber</h1>
			<p class="slogan">Full-Stack Engineer | UI/UX Designer</p>
			<p class="location">Helena, Montana</p>
			<div class="container-about">
				<h2>About me</h2>
				<p>From licking stamps to directing statewide projects, I enjoy a wide range of passions. <br> <br> <br> Web accessibility is one of my most passionate - from Section 508 to AAA WCAG 2.2 standards. <br> <br> <br> This site contains best practices I employ, inspirations, and my proudest works. </p>
			</div>
		</div>
		<div class="container">
			<a href="#" class="logo"><Chase/></a>
			<h1 class="name">Chase Alber</h1>
			<p class="slogan">Full-Stack Engineer | UI/UX Designer</p>
			<p class="location">Helena, Montana</p>
			<div class="container-about">
				<h2>About me</h2>
				<p>From licking stamps to directing statewide projects, I enjoy a wide range of passions. <br> <br> <br> Web accessibility is one of my most passionate - from Section 508 to AAA WCAG 2.2 standards. <br> <br> <br> This site contains best practices I employ, inspirations, and my proudest works. </p>
			</div>
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
		margin-bottom: 1em;
	}
	.container > h1 {

		margin: 0.2em;
	}
	.container > p {

		margin-top: 0.5em;

	}
	.container-about {
		align-self: center;
		text-align: center;
		height: 60vh;
		padding: 2rem 0rem;
		margin-bottom: 2rem;
	}
	.container-about > h2 {
		padding: 0.5em 0;
		margin: 0em 2em;
		background-color: var(--black);
		border-radius: 25px;
		color: var(--light-parch);
	}
	.container-about > p {
		margin: 2em 0.8em;
		padding: 1.5em;
		word-wrap: break-word;
		color: var(--brown);
		opacity: 90%;
	}
	.name {
		font-size: 2.4rem;
		color: var(--brown);
		opacity: 90%;
	}
	.slogan {
		font-size: 1em;
		font-weight: 300;
		font-family: 'Goth-Med';
		color: var(--brown);
		opacity: 90%;
	}

	.location {
		font-family: 'Goth-Med';
		color: var(--brown);
		opacity: 90%;
	}
	@media (min-width: 905px) {
		.home-article {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		margin-top: 10vh;
	}
		.container-about {
			margin: 0 auto;
			width: 100%;
			align-self: center;
			text-align: center;
			max-height: 35vh;
			padding: 1rem;
			border-radius: 50px;
			margin-bottom: 2rem;
		}
		.container-about > h2 {
		margin: 0.2em;
		color: var(--ivory);
		}
		.container-about > p {
			margin: 0.5em auto;
			padding: 0.5em;
			color: var(--black);
			border-radius: 25px;
			width: 100%;
		}
	}
</style>