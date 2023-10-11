<nav>
    <div class="nav-item">Test</div>
    <div class="nav-item">Test</div>
    <div class="nav-item">Test</div>
    <div class="nav-item">Test</div>
    <div class="nav-item">Test</div>
</nav>

<div id="design">
    <div id="design-inner">
        <div class="top-area">
            <h1>ChaseAlber</h1>
            <h2>Sub-header</h2>
            <div class="icons">icons</div>
            <div class="tag-warn">label</div>
            <div class="icons">icon</div>
        </div>
        <div class="mid-area">
            <div><b>MODEL</b> 311202</div>
            <div><b>MODEL</b> 311202</div>
            <p></p>
        </div>
        <div class="bot-area">
            <div class="caution-box"></div>
            <ul>
                <li></li>
                <li></li>
            </ul>
        </div>
    </div> 
</div>

<section>
    <slot/>
</section>

<style>
    h1{
        margin: 0;
    }
    h2 {
        margin: 0;
    }
    #design {
        background-color: var(--ivory);
        width: 20%;
        height: 100%;
        position: absolute;
        left: 0;
        top: 0;
        display: flex;
        flex-direction: column;
    }
    #design-inner {
        width: 90%;
        height: 100%;
        display: flex;
        flex-direction: column;
        margin: 10% 10%;
    }
    .top-area {
        width: 100%;
        height: 30%;
        display: flex;
        flex-direction: column;
        justify-content: start;
        align-items: start;
    }
    .mid-area {
        width: 100%;
        height: 40%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: start;
    }
    .bot-area {
        width: 100%;
        height: 30%;
        display: flex;
        flex-direction: column;
        justify-content: end;
        align-items: start;
    }
    nav {
        background-color: var(--ivory);
        width: 80%;
        height: 10%;
        position: absolute;
        top: 0;
        right: 0;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }
    .nav-item {
        margin-top: 1%;
        height: 40%;
        width: 15%;
        border: black 2px dotted;
    }
    section {
        width: 80%;
        height: 90%;
        background-color: var(--ivory);
        position: absolute;
        right: 0;
        bottom: 0;
        display: flex;   
    }

    :root{
        --ivory: #FAF9F1;
    }
</style>