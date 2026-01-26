



<main class="container">
    <!-- display area -->
    <div class="timer-display">
        00:00'00"000
    </div>

    <!-- button group -->
    <div class="button-group">
        <button class="btn-start">START/STOP</button>
        <button class="btn-lap">LAP</button>
        <button class="btn-reset">RESET</button>
    </div>

    <!-- lap board -->
    <div class="lap-board">
        <span class="col-time">LAP TIME</span>
        <span class="col-diff">DIFF</span>
    </div>

    <!-- lap list content -->
    <div class="lap-list">
        <div class="lap-item">
            <span class="col-time">XX:XX'XX"XXX</span>
            <span class="col-diff">+ XX:XX'XX"XXX</span>
        </div>
    </div>

</main>

<style>
    /* global css */
    :global(html), :global(body) {
        margin: 0;
        padding: 0;
        overflow: hidden;
        overscroll-behavior: none;
    }

    main {
        display: flex;
        max-width: 320pt;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        min-height: 100dvh;
        margin: 0;
        margin-left: auto;
        margin-right: auto;
    }

    .timer-display {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 56pt;
        font-size: x-large;
        border-style: solid;
        border-width: 1.5px;
        border-color: gray;
        margin-bottom: 0.5rem;
    }

    .button-group {
        width: 100%;
        display: flex;
        flex-flow: row;
        justify-content: space-around;
        height: 44px;
        margin: 0;
        margin-top: 0.5rem;
        margin-bottom: 0.5rem;
    }

    button {
        border-radius: 12rem;
        min-width: 55px;
        padding-left: 24px;
        padding-right: 24px;
        font-weight: bold;
        font-size: 1rem;
    }

    .btn-start {
        background-color: #4bb023;
        color: black;
    }

    .btn-lap {
        background-color: lightgray;
        color: black;
    }

    .btn-reset {
        background-color: #b5350b;
        color: white;
    }

    .lap-board, .lap-list {
        width: 100%;
        display: flex;
        justify-content: space-evenly;
        flex-flow: row;
        text-align: left;
    }

    .lap-board {
        border-bottom-style: solid;
        border-width: 1px;
        padding-bottom: 0.5rem;
        padding-top: 0.5rem;
    }

    .lap-item {
        width: 100%;
        display: flex;
        justify-content: space-evenly;
        flex-flow: row;
        text-align: left;
        padding-top: 0.5rem;
    }

    .col-time {
        flex-grow: 1;
        width: 100%;
        margin: 0;
        margin-right: 10px;
    }

    .col-diff {
        flex-grow: 1;
        width: 100%;
        margin: 0;
        margin-left: 10px;
    }

</style>