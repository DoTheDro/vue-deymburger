<script>
    import logo from '../assets/images/site-logo.png'
    import imageBig from '../assets/images/hero-image.png'
    import imageSmall from '../assets/images/hero-image-mobile.png'


    export default {
        data() {
            return {
                logo: logo,
                imageBig: imageBig,
                imageSmall: imageSmall,
                show: false
            }
        },
        methods: {
            showForm() {
                console.log('button clicked')
            }
        }
    }
</script>

<template>
    <div>
        <div>
            <div class="float-left">
                <a href="/">
                    <img class="mt-2 ml-3 w-20" :src="logo" alt="Website Logo">
                </a>
            </div>

            <div>
                <button class="mt-4 mr-4 px-2 py-2 border-2 text-gray-300 rounded-lg border-gray-300 float-right" @click="showForm">Order Now!</button>
            </div>
        </div>
        <div class="-mb-20">
            <img class="m-auto" :src="imageSmall" alt="Burger Image">
        </div>
    </div>
</template>