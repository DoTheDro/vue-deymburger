<script>
    import aboutImage from '../assets/images/about-us-image.png'

    export default {
        data() {
            return {
                image: aboutImage,
                sectionHeader: 'About Us',
                content: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. A consequuntur impedit corrupti deserunt obcaecati totam aspernatur amet, officiis repellat aperiam.',
                franchises: 9,
                customers: 87
            }
        }
    }
</script>

<template>
    <div class="py-10" id="about"></div>
    <div data-aos="fade-up"
        data-aos-duration="700"
        data-aos-once="true"    
    class="px-4 pb-16 flex flex-col gap-12 sm:max-w-7xl sm:m-auto">
        <h2 class="text-4xl text-yellow-400 font-bold">{{ sectionHeader }}</h2>
        <p class="text-lg text-gray-200 text-center sm:text-left sm:text-xl">{{ content }}</p>
        <div class="flex justify-center gap-10">
            <div class="flex flex-col text-center gap-1">
                <p class="text-xl text-yellow-400 font-semibold sm:text-2xl">{{ franchises }}</p>
                <p class="text-lg text-yellow-400 font-semibold sm:text-xl">Franchises</p>
            </div>

            <div class="flex flex-col text-center gap-1">
                <p class="text-xl text-yellow-400 font-semibold sm:text-2xl">{{ customers }}</p>
                <p class="text-lg text-yellow-400 font-semibold sm:text-xl">Burgers</p>
            </div>
        </div>
    </div>
</template>