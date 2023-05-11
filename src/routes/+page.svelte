<script>
    import Card from './Card.svelte'

    const profile_image = { src: './src/lib/profile_pic.jpg', alt: 'Minh Nguyen' }
</script>

<div class="flex-container">
    <Card title="Minh Nguyen" {...profile_image} />
    <Card title="About Me" text="Hello, world! I'm an incoming freshman at the University of Texas at Dallas that's majoring in computer engineering!" />
</div>

<style lang="scss">
    .flex-container {
        display: flex;
        gap: 1em;
    }
</style>