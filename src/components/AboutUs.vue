<script>
    import aboutImage from '../assets/images/about-us-image.png'

    export default {
        data() {
            return {
                text: 'About Us sample text',
                image: aboutImage
            }
        }
    }
</script>

<template>
    <h1 class="text-2xl text-gray-400">{{ text }}</h1>
</template>