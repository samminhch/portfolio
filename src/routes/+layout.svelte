<div class="container">
    <slot />
</div>

<style>
    @import '../colors.scss';
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
        background-color: var(--color-background);
        background-size: 40px 40px;

        background-image: linear-gradient(to right, var(--color-background-accent) 1px, transparent 1px),
            linear-gradient(to bottom, var(--color-background-accent) 1px, transparent 1px);

        height: 100vh;
    }

    .container {
        max-width: calc(100% - 4em);
        margin-inline: auto;
        margin-top: 2em;
        margin-bottom: 2em;
    }
</style>
