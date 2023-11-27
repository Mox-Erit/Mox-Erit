<script>
// @ts-nocheck

    export let title;
    export let clientDesc;
	export let image;
	export let imageDesc;
</script>

            <div class="portfolio-item">
				<img src={image} alt={imageDesc}>
                <title>&#x2022; {title}</title>
                <p>{clientDesc}</p>
            </div>


<style>
	img {
		border-top-right-radius: 50px;
		border-top-left-radius: 50px;
		width: 100%;
		height: auto;
	}
	.portfolio-item {
		display: flex;
		align-items: start;
		justify-content: start;
		flex-direction: column;
		flex: 1;
	}
	
	title {
		margin: 1.4em 0.8em 0.4em 0.8em;
		display: flex;
		color: var(--parchment);
		background-color: var(--black);
		padding: 0.4em 1em;
		border: 1px solid var(--black);
		border-radius: 25px;
	}
	p {
		margin-left: 0.8em;
		margin-bottom: 1.2em;
		font-size: 1em;
		display: flex;
		color: var(--black);
		display: flex;
		padding: 1em;
	}
</style>