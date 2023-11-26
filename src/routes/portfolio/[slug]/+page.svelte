<script>
    /** @type {import('./$types').PageData} */
	export let data;
    import Image from "$lib/assets/uibanner.png";



</script>


<div class="page-wrapper">
    <div class="portfolio-page">
        <div class="banner-top">&#x2022; RECORDING</div>
        <img  class="banner" src={Image} alt="">
        <h1>{data.posts[0].title}</h1>
        <div class="line"></div>
        <article>{@html data.posts[0].content}</article>
    </div>
</div>




<style>
.page-wrapper {
    
    display: flex;
    align-items: center;
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
.banner-top {
    font-size: 0.8rem;
    display: flex;
    color: var(--tech-orange);

}
.banner {
    margin: 1em 0 1.5em 0;
    display: flex;
}
h1 {
    font-family: 'Goth-Med';
    color: var(--brown);
    opacity: 90%;
}
.line {
    opacity: 90%;
    width: 100%;
    height: 0.2em;
    background-color: var(--brown);
    margin: 1.5em 0 1em 0;
}
article {
    opacity: 90%;
    display: flex;
    font-size: 1.2em;
    line-height: 1.5em;
    color: var(--brown);
    margin: 1em 0;
}
</style>