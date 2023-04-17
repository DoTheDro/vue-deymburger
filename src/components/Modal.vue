<script>
    export default {
        data() {
            return {
                sectionHeader: 'Order Form'
            }
        },
        methods: {
            closeModal() {
                this.$emit('close')
                console.log('test')
            }
        }
    }
</script>

<template>
    <div data-aos="fade-down"
        data-aos-duration="200"
        class="w-full h-screen bg-black bg-opacity-80 top-0 left-0 fixed flex items-center justify-center z-40 px-4" @click.self="closeModal">
        <div class="h-56 w-full bg-gray-100 flex flex-col justify-evenly rounded-lg p-4 max-w-md">
            <h4 class="text-4xl text-yellow-400 font-bold text-center">{{ sectionHeader }}</h4>
            <p class="text-lg text-gray-950 text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat tempore laborum officia nobis. Magni, magnam aliquam ad optio veritatis voluptas!</p>
        </div>
    </div>
</template>