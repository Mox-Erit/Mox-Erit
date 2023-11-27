<script>
    /** @type {import('./$types').PageData} */
	export let data;
    import Image from "$lib/assets/uibanner.png";
    import { fade } from 'svelte/transition';
</script>


<div class="page-wrapper" in:fade>
    <div class="portfolio-page">
        <div class="banner-top">&#x2022; jQuery &#x2022; Bootstrap 5 &#x2022; CascadeCMS</div>
        <img  class="banner" src={Image} alt="">
        <h1>{data.posts[0].title}</h1>
        <div class="line"></div>
        <p>https://livestock.com</p>
        <article>{@html data.posts[0].content}</article>
    </div>
</div>




<style>
h1 {
    font-size: 1.5em;
    margin-top: 0.5em;
    color: var(--brown);
    opacity: 90%;
}
p {
    margin: 0 0 0.3em 0;
    font-family: 'Goth-Med';
}
.page-wrapper { 
    display: flex;
    align-items: center;
    height: 100%;
    margin-top: 10vh;

}
.portfolio-page{
    margin-top: 1em;
    padding: 1em;
    display: flex;
    flex-direction: column;
    width: 100%;
}
.banner-top {
    font-size: 1rem;
    display: flex;
    color: var(--tech-orange);

}
.banner {
    margin: 1em 0 1.5em 0;
    display: flex;
}
.line {
    opacity: 80%;
    width: 100%;
    height: 0.2em;
    background-color: var(--brown);
    margin: 0.4em 0 1em 0;
}
article {
    opacity: 90%;
    display: flex;
    font-size: 1.2em;
    line-height: 1.5em;
    color: var(--brown);
    margin: 1em 0;
    font-family: 'Goth-Med';
}

@media (min-width: 905px) {

	.page-wrapper {
        padding: 1.5rem;
    }

    .portfolio-page{
    box-shadow: 0em 0em 1em 0.2em var(--brown);
    background: var(--parchment);
    padding: 3rem;
    display: flex;
    flex-direction: column;
    width: 100%;
    margin: 0 auto;
}

.portfolio-page{
    padding: 3rem;
    display: flex;
    flex-direction: column;
    width: 100%;
    margin: 0 auto;
}
	
	}
</style>