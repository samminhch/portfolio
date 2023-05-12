<div class="container">
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
        line-height: 1.5;
    }

    :global(img) {
        max-width: 100%;
        display: block;
    }

    :global(body) {
        background-color: #d9ead3;
        background-size: 40px 40px;

        background-image: linear-gradient(to right, #333e36 1px, transparent 1px),
            linear-gradient(to bottom, #333e36 1px, transparent 1px);

        border: 1px solid #333e36;
        height: 100vh;
    }

    .container {
        margin: 2em;
    }
</style>
