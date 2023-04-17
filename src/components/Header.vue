<script>
    import logo from '../assets/images/site-logo.png'

    export default {
        data() {
            return {
                logo: logo,
                header: 'Lorem ipsum dolor sit amet consectetur adipisicing.',
                content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa nemo doloremque repudiandae facilis, quod dignissimos id iusto praesentium quisquam tempora atque in magni vero exercitationem?'
            }
        }
    }
</script>

<template>
    <div class="bg-gray-100 -mt-3 mx-4 pt-16 box-shadow rounded sm:pt-0 sm:w-2/4 sm:bg-gray-800 sm:absolute sm:z-10 sm:m-0 sm:rounded-none sm:h-full sm:top-0 sm:flex sm:flex-col sm:rounded-br-md sm:items-end">
        <div class="p-4 flex flex-col gap-6 sm:max-w-screen-sm sm:h-full sm:justify-between md:justify-center md:gap-12 lg:relative">
            <div class="hidden sm:flex sm:justify-between sm:items-center lg:absolute lg:top-0 lg:mt-4">
                <div class="flex items-center gap-3">
                    <img class="w-20 inline-block" :src="logo" alt="Site Logo">
                    <p class="text-xl text-yellow-400">Deymburger</p>
                </div>
            </div>
            <div class="flex flex-col gap-4 lg:h-4/5 lg:justify-end lg:gap-16">
                <h1 class="text-2xl text-gray-950 font-bold sm:text-4xl sm:text-yellow-400">{{ header }}</h1>
                <p class="text-base sm:text-lg sm:text-gray-100">{{ content }}</p>
                <div class="">
                    <a class="text-base p-2 border-gray-900 border-2 rounded-md flex justify-center w-32 sm:text-gray-100 sm:border-gray-100" href="">How It Works</a>
                </div>
            </div>
        </div>
    </div>
</template>