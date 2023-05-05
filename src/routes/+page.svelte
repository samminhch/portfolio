<script>
    import Card from './Card.svelte'

    const profile_image = { src: './src/lib/profile_pic.jpg', alt: 'Minh Nguyen' }
</script>

<Card {...profile_image} />
