<script lang="ts">
    // let the image path be specified by parent
    export let title: string = ''
    export let src: string = ''
    export let alt: string = ''
    export let text: string = ''
</script>

<div class="card">
    {#if title != ''}
        <h2>{title}</h2>
    {/if}

    {#if src != '' && alt != ''}
        <img src={src} alt={alt} />
    {/if}

    {#if text != ''}
        <p>{text}</p>
    {/if}
</div>

<style lang="scss">
    .card {
        --radius: 12px;
        --border-color: black;
        --blur-color: rgba(0, 0, 0, 0.2);
        --element-background-color: rgb(228, 229, 232);

        background-color: white;
        width: 16em;
        height: -moz-fit-content;
        height: fit-content;
        padding: 0.5em 2em 1.5em;

        border: 3px solid var(--border-color);
        border-radius: var(--radius);

        box-shadow: 0 4px 8px 0 var(--blur-color), 0 6px 20px 0 var(--blur-color);

        img {
            width: 100%;
            border-radius: var(--radius);
            border: 2px solid var(--border-color);
        }

        h2 {
            padding: 0.125rem 0.5rem;
            background-color: var(--element-background-color);
            border-radius: calc(var(--radius) / 2);
            box-shadow: 0 4px 8px 0 var(--blur-color) inset;
        }

        p {
            background-color: var(--element-background-color);
            padding: 0.25rem;

            border: 2px solid var(--border-color);
            border-radius: calc(var(--radius) / 2);
        }
    }
</style>
