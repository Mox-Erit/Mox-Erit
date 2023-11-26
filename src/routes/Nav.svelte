<script>
    import { page } from '$app/stores';

    let path;

    $: path = $page.url.pathname;
</script>
<header>
    <a href="#" class="logo">CA</a>
    <input type="checkbox" class="nav" id="nav">
</header>
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
        <li aria-current={$page.url.pathname === '/gallery' ? 'page' : undefined}>
            <a href="/gallery">Gallery</a>
        </li>
    </ul>
</nav>

<style>
    nav {
       
    } 
    ul {
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        list-style: none;
    }
    li {
        width: 10vw;
        border: black 2px dotted;
        display: flex;
        justify-content: center;
	}
    nav a {
        text-decoration: none;
        text-transform: uppercase;
        letter-spacing: 0.05em;
    }
</style>