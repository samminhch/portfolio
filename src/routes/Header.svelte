<script lang="ts">
    export let title: string
</script>

<header>
    <h1>{title}</h1>
</header>

<style lang="scss">
    @import '../colors.scss';
    header {
        --radius: 12px;
        --blur-color: rgba(0, 0, 0, 0.2);

        background: var(--color-foreground);
        border: 3px solid black;
        border-radius: var(--radius);
        padding: 0em 2em;

        display: flex;
        align-items: center;

        h1 {
            margin: .25em auto;
            background: var(--color-foreground-accent);
            width: -moz-fit-content;
            width: fit-content;
            padding: 0em 0.5em;
            box-shadow: 0 4px 8px 0 var(--blur-color) inset;
            border-radius: calc(var(--radius) / 2);
        }
    }
</style>
