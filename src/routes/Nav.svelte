<script>
    import { page } from '$app/stores';

    let path;

    $: path = $page.url.pathname;
</script>
<header class="header">
    <!-- Logo -->
    <a href="#" class="logo">CA</a>
    <!-- Hamburger icon -->
    <input type="checkbox" class="side-nav" id="side-nav"/>
    <label for="side-nav" class="hamb"><span class="hamb-line"></span></label>
    <!-- Navigation Menu -->
    <nav class="nav">
        <ul class="menu">
            <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
                <a href="/">Home</a>           
            </li>
            <li aria-current={$page.url.pathname === '/portfolio' ? 'page' : undefined}>
                <a href="/portfolio">Portfolio</a>
            </li>
            <li aria-current={$page.url.pathname === '/accessibility' ? 'page' : undefined}>
                <a href="/accessibility">Accessibility</a>
            </li>
            <li aria-current={$page.url.pathname === '/inspiration' ? 'page' : undefined}>
                <a href="/inspiration">Inspiration</a>
            </li>
        </ul>
    </nav>
</header>


<style>
    .header {
    z-index: 2;
    position: sticky;
    top: 0px;
    width: 100%;
    }
    .logo {
        display: none;
    }
    .nav {
        z-index: 2;
        width: 100%;
        height: 100vh;
        top: 0;
        position: absolute;
        background-color: var(--black);
        overflow: hidden;
        max-height: 0;
        transition: max-height .15s ease-out;
    } 
    .menu a {
    display: block;
    padding: 36px;
    color: var(--ivory);
    }
    .menu a:hover {
    background-color: var(--tech-orange);
    transition: all .2s ease-out;
    }
    .menu {
        z-index: 3;
    }
    /* Menu Icon */
    .hamb {
        z-index: 3;
        cursor: pointer;
        float: right;
        padding: 40px;
    }/* Style label tag */
    .hamb-line {
        z-index: 3;
        background: var(--yellow);
        display: block;
        height: 7px;
        position: relative;
        width: 36px;

    } /* Style span tag */
    .hamb-line::before {
        z-index: 3;
        background: var(--auburn);
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all .2s ease-out;
        width: 100%;
    
    }
    .hamb-line::after {
        z-index: 3;
        background: var(--teal);
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all .2s ease-out;
        width: 100%;
    }
    .hamb-line::before {
        top: 12px;
    }
    .hamb-line::after {
        top: -12px;
    }
    .side-nav {
        display: none;
    } /* Hide checkbox */
    /* Toggle menu icon */
    .side-nav:checked ~ nav{
        max-height: 368px;
        
    }
    .side-nav:checked ~ .hamb .hamb-line {
        background: transparent;
    }
    .side-nav:checked ~ .hamb .hamb-line::before {
        transform: rotate(-45deg);
        top:0;
    }
    .side-nav:checked ~ .hamb .hamb-line::after {
        transform: rotate(45deg);
        top:0;
    }
    /* Responsiveness */
    @media (min-width: 905px) {
        .nav{
            width: 100%;
            height: 10vh;
            max-height: none;
            top: 0px;
            position: relative;
            float: right;
            width: fit-content;
            background-color: transparent;
        }
        .logo {
            display: inline-block;
            font-size: 4.6rem;
            padding: 0 0.3em;
        }
        .menu li{
            float: left;
        }
        .menu a {
        display: block;
        padding: 35px;
        color: var(--ivory);
        }
        .menu a:hover{
            background-color: transparent;
            color: var(--tech-orange);

        }

        .hamb{
            display: none;
        }
        .header {
            min-height: 10vh;
            background-color: var(--black);
            position: sticky;
            top: 0px;
            width: 100%;
        }
    }
    /* ul {
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
    } */
</style>