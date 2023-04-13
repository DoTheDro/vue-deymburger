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
    <div class="bg-gray-100 -mt-3 mx-4 pt-16 box-shadow rounded">
        <div class="p-4 flex flex-col gap-6">
            <div class="hidden">
                <img class="" :src="logo" alt="Site Logo">
                <a href="">How It Works</a>
            </div>
            <h1 class="text-2xl text-gray-950 font-bold">Lorem ipsum dolor sit amet consectetur adipisicing.</h1>
            <p class="text-baseg">Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa nemo doloremque repudiandae facilis, quod dignissimos id iusto praesentium quisquam tempora atque in magni vero exercitationem?</p>
            <div>
                <a class="text-base p-2 border-gray-900 border-2 rounded-md flex justify-center w-32" href="">How It Works</a>
            </div>
        </div>
    </div>
    <h1 class="text-2xl text-gray-100">{{ text }}</h1>
</template>