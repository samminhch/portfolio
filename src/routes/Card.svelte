<script>
    // let the image path be specified by parent
    let source = { path: './src/lib/profile_pic.jpg', description: 'Minh Nguyen' }
</script>

<div class="card">
    <h2>Minh Nguyen</h2>
    <img src={source.path} alt={source.description} />
</div>

<style lang="scss">
    .card {
        --radius: 12px;
        --border-color: black;
        --blur-color: rgba(0, 0, 0, 0.2);

        background-color: white;
        width: 16em;
        padding: 0.5em 2em 1em;

        border: 3px solid var(--border-color);
        border-radius: var(--radius);

        box-shadow: 0 4px 8px 0 var(--blur-color), 0 6px 20px 0 var(--blur-color);

        img {
            width: 100%;
            border-radius: calc(var(--radius) * 2);
            box-shadow: 0 4px 8px 0 var(--blur-color) inset;
        }

        h2 {
            padding: 0.125rem 0.5rem; 
            background-color: rgb(228, 229, 232);
            border-radius: calc(var(--radius) / 2);
            box-shadow: 0 4px 8px 0 var(--blur-color) inset;
        }
    }
</style>
