<script>
    import { fade } from 'svelte/transition';
    import './styles.css';
    import { page } from '$app/stores';
    import SideMenu from './SideMenu.svelte';
    import Nav from './Nav.svelte';
</script>
<svelte:head>
    <title>{$page.url.pathname.replaceAll('-', ' ')}</title>
</svelte:head>
    <!-- <aside>
        <SideMenu />
    </aside> -->
<main in:fade>
    <Nav  />

    <slot />
</main>



   


<style>
main {
  overflow-y: auto;
}
</style>