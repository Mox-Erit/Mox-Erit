<script>
// @ts-nocheck
    import LeftArrow from '../components/left-arrow.svelte';
    import Vert from '../components/vertical-lonetrail.svelte';
    import Home from '../components/home-icon.svelte';
    import { page } from '$app/stores';

    let path;

    $: path = $page.url.pathname;
</script>



<div class="aside-container">
    <div class="item-top">
        <div class="item-top-left">
            <button onclick="history.back()"><Vert/><LeftArrow/></button>
        </div>
        <div class="item-top-right"><button onclick="history.go(-1)"><Home/></button></div>
    </div>
    <div class="item-mid"></div>
    <div class="item-bottom"></div>
</div>


<style>
.aside-container {
    position: absolute;
    top: 84px;
}
.item-top {
   transition: all 0.2s ease-in-out;
   box-shadow: 0em 0em 0.7em 0.1em var(--brown);
   background: var(--black);
   display: flex;
   min-height: 1vh;
} 
.item-top:hover {
    transition: all 0.2s ease-in-out;
    box-shadow: 0em 0em 1em 0.2em var(--brown);
}
.item-top-left {
    flex: 1;
    background: var(--black);
    border-right: 3px solid black;
}
button {
    transition: all 0.2s ease-in-out;
    background: var(--black);
    border: none;
    cursor: pointer;
    width: 100%;
    height: 100%;
    display: flex;
    justify-items: center;
    align-items: center;
    padding: 0;
}
button:hover {
    transition: all 0.2s ease-in-out;
    box-shadow: 0em 0em 1em 0.2em var(--brown);
}
.item-top-right {
    flex: 2 1 0;
    display: flex;
}

.item-mid {
    min-height: 25vh;
    background: var(--black);
    margin: 4em 0;
} 
.item-bottom {
    background: var(--black);
   margin-top: 15em;
   min-height: 30vh;
} 
</style>