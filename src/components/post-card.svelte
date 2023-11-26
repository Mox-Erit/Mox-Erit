<script>
// @ts-nocheck

    export let title;
    export let client;
    export let clientDesc;
</script>

            <div class="port-item-left">
                <title>&#x2022; Project Title</title>
                <p>{title}</p>
            </div>
            <div class="port-item-right">
                <title>Client</title>
                <p>{client} <br/> {clientDesc}</p>
            </div>
            <div class="port-item-end">
                <title>Workflow</title>
                <div class="end-item-group">
                    <div class="end-item"></div>
                    <div class="end-item"></div>
                    <div class="end-item"></div>
                </div>
            </div>


<style>
    .portfolio-item:hover {
		transition: all 0.2s ease-in-out;
		box-shadow: 0em 0.5em 1em 0 var(--black);
		scale: 1.009;
	}
	.portfolio-item {
		display: flex;
		flex-grow: 1;
		background: var(--parchment);
		margin-bottom: 1rem;
		min-height: 20px;
		box-shadow: 0em 0.2em 0.7em 0 var(--black);
	}
	.port-item-left {
		display: flex;
		align-items: start;
		justify-content: start;
		flex-direction: column;
		flex: 2;
	}
	.port-item-right {
		display: flex;
		align-items: start;
		justify-content: start;
		flex-direction: column;
		flex: 1;
	}
	.port-item-end {
		display: flex;
		align-items: center;
		justify-content: start;
		flex-direction: column;
		flex: 1;
	}
	.end-item-group {
		margin-top: 0.5em;
		display: flex;
		flex-wrap: wrap;
	}
	.end-item-group > div {
		flex: 100%;
	}
	.end-item {
		justify-content: center;
		min-width: 100%;
		min-height: 50%;
		display: flex;
		background: var(--tech-orange);
		margin: 0.2em;
	}
	title {
		margin: 0.8em 0 0 3em;
		display: flex;
		color: var(--parchment);
		background-color: var(--black);
		padding: 0.3em 1.5em;
		border: 1px solid var(--black);
		border-radius: 25px;
	}
	.port-item-end > title {
		margin: 0.8em 0 0 0em;
	}
	p {
		margin-left: 1.8em;
		font-size: 1.5em;
		font-weight: bold;
		letter-spacing: -1px;
		display: flex;
		color: var(--black);
		display: flex;
		padding: 0.3em 1em;
		border-radius: 25px;
	}
	.port-item-right > p {
		margin-left: 1.8em;
		font-size: 1.2em;
		font-weight: bold;
		letter-spacing: -1px;
		display: flex;
		color: var(--black);
		display: flex;
		padding: 0.3em 0.1em;
		border-radius: 25px;
	}
	.portfolio-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;

	}
</style>