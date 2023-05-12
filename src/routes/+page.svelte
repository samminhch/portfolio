<script>
    const profile_image = { src: './src/lib/profile_pic.jpg', alt: 'Minh Nguyen' }
</script>

<div class="flex-container">
    <div class="card profile-image">
        <h2>Minh Nguyen</h2>
        <img src={profile_image.src} alt={profile_image.alt} />
    </div>
    <div class="card">
        <h2>About Me</h2>
        <p>wow it's me minh bow down to me mortal</p>
    </div>
</div>

<style lang="scss">
    .flex-container {
        display: flex;
        gap: 1em;
    }

    .card {
        --radius: 12px;
        --border-color: black;
        --blur-color: rgba(0, 0, 0, 0.2);
        --element-background-color: rgb(228, 229, 232);

        background-color: white;
        max-width: 32em;
        height: -moz-fit-content;
        height: fit-content;
        padding: 0.5em 2em 1.5em;

        border: 3px solid var(--border-color);
        border-radius: var(--radius);

        box-shadow: 0 4px 8px 0 var(--blur-color), 0 6px 20px 0 var(--blur-color);

        img {
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

    .profile-image {
        max-width: 16em;
    }
</style>
