<script>
    import { page } from '$app/stores';
</script>
<nav>
    <ul>
        <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
            <a href="/">Home</a>           
        </li>
        <li aria-current={$page.url.pathname === '/portfolio' ? 'page' : undefined}>
            <a href="/portfolio">Portfolio</a>
        </li>
        <li aria-current={$page.url.pathname === '/accessibility' ? 'page' : undefined}>
            <a href="/accessibility">Accessibility</a>
        </li>
        <li aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
            <a href="/contact">Contact</a>
        </li>
        <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
            <a href="/about">About</a>
        </li>
    </ul>
</nav>

<style>
    nav {
        background-color: var(--ivory);
        width: 85%;
        height: 10%;
        position: absolute;
        top: 0;
        right: 0;
        display: flex;
        align-items: center;
    }
    ul {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
        list-style: none;
        background-size: contain;
    }
    li {
		position: relative;
		height: 100%;
        margin-top: 1%;
        height: 40%;
        width: 15%;
        border: black 2px dotted;
        display: flex;
        justify-content: center;
	}
    nav a {
        display: flex;
        align-items: center;
        text-decoration: none;
        text-transform: uppercase;
        letter-spacing: 0.05em;

    }
</style>