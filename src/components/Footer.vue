<script>
    import logo from '../assets/images/site-logo.png'

    export default {
        data() {
            return {
                logo: logo
            }
        }
    }
</script>

<template>
    <div class="px-4 pb-8 pt-4 bg-gray-700">
        <div class="flex flex-col gap-8">
            <div class="">
                <a class="flex flex-row justify-center items-center gap-4" href="/">
                    <div class="w-20">
                        <img :src="logo" alt="Site Logo">
                    </div>
                    <p class="text-2xl text-yellow-400 font-bold">Deymburger</p>
                </a>
            </div>
            <div class="flex flex-col items-center gap-4">
                <a class="text-xl text-yellow-400 font-semibold" href="/">Home</a>
                <a class="text-xl text-yellow-400 font-semibold" href="#about">About Us</a>
                <a class="text-xl text-yellow-400 font-semibold" href="#products">Our Products</a>
                <a class="text-xl text-yellow-400 font-semibold" href="#menu">Menu</a>
                <a class="text-xl text-yellow-400 font-semibold" href="#procedure">Procedure</a>
            </div>
            <p class="text-base text-center text-gray-100">Created and Built by Andrew Buhat</p>
        </div>
    </div>
</template>