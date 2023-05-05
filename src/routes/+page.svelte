<script>
    import Card from './Card.svelte'

    const profile_image = { src: './src/lib/profile_pic.jpg', alt: 'Minh Nguyen' }
</script>

<Card title='Minh Nguyen' {...profile_image} />
<Card title='About Me' text='Hello, world!'/>
