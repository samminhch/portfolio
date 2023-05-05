<div class="background">
    <slot />
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Bree+Serif&display=swap');

    :global(h1, h2) {
        font-family: 'Bree Serif', serif;
        font-weight: 400;
    }

    :global(p) {
        font-family: 'Atkinson Hyperlegible', sans-serif;
    }

    .background {
        /* make this take up the whole page */
        min-height: 100vh;
        min-width: 100vw;

        padding: 2em;
        /* make this background a grid */
        background-color: #d9ead3;
        background-size: 40px 40px;

        background-image: linear-gradient(to right, #333e36 1px, transparent 1px),
            linear-gradient(to bottom, #333e36 1px, transparent 1px);
        border: 1px solid #333e36;
    }
</style>
