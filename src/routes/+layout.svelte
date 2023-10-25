<script>
    import Nav from './Nav.svelte';
    import Menu from './Menu.svelte';
    import './styles.css';
</script>

<div>
    <Nav />

    <Menu />

    <main>
        <slot />
    </main>
</div>

<style>
    main {
        width: 85%;
        height: 90%;
        /* background-color: var(--ivory); */
        background-color: grey;
        position: absolute;
        right: 0;
        bottom: 0;
        display: flex;   
    }
</style>