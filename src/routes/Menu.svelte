<div id="left-menu">
    <div id="left-menu-inner">
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

<style>
    #left-menu {
        /* background-color: var(--ivory); */
        background-color: yellow;
        width: 15%;
        height: 100%;
        position: absolute;
        left: 0;
        top: 0;
        display: flex;
        flex-direction: column;
    }
    #left-menu-inner {
        height: 100%;
        display: flex;
        flex-direction: column;
        margin: 10% 20%;
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
</style>