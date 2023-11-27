<script>
    import Icon from '../../Icon.svelte';
</script>
<svelte:head>
    <title>Gallery</title>
    <meta name="description" content="Get to know more about me and my process, or don't. You have free will and I would like to remind you of that." />
</svelte:head>
<div id="left-menu">
    <div id="left-menu-inner">
        <div class="top-area">           
            <h1><Icon name="test1" />Gallery</h1>
            <span><Icon name="test2" />Collection of my stamps and 3D models</span>
            <br />
            <span><Icon name="test1" /><Icon name="test1" /></span>
            <div class='text-block'></div>
            <span style="margin-top: 0.1em;"><Icon name="test1" /></span>
        </div>
        <div class="mid-area">
            <span><b>MODEL</b><span style="margin-left: 2em;">311202</span></span>
            <span><b>SERIAL</b><span style="margin-left: 1em;">00000026</span></span>
        </div>
        <div class="bot-area">
            <div class="caution-box">

            </div>
            <ul>
                <li></li>
                <li></li>
            </ul>
        </div>
    </div> 
</div>

<main class="content">
    
</main>

<style>
    .text-block {
        height: 9em;
        width: 6em;
        border: 2px solid black;
    }

    .caution-box {
        height: 6em;
        width: 12em;
        border: 2px solid black;
    }

    .content {
        display: flex;
        flex-direction: row;
    }
</style>