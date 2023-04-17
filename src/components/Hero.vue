<script>
    import logo from '../assets/images/site-logo.png'
    import imageBig from '../assets/images/hero-image.png'
    import imageSmall from '../assets/images/hero-image-mobile.png'
    import Modal from './Modal.vue'
import { Teleport } from 'vue'


    export default {
        components: { Modal, Teleport },
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
                this.show = !this.show
            },
            closeForm() {
                this.show = !this.show
            }
        }
    }
</script>

<template>
    <Teleport v-if="show" to="#modal">
            <Modal @close="closeForm" />
    </Teleport>
    <div data-aos="fade-left"
        data-aos-duration="700"
        data-aos-once="true"    
    class="sm:w-full sm:max-w-7xl sm:m-auto sm:pt-5">
        <div>
            <div class="float-left sm:hidden">
                <a href="/">
                    <img class="mt-2 ml-3 w-20" :src="logo" alt="Website Logo">
                </a>
            </div>

            <div>
                <button class="mt-4 mr-4 px-2 py-2 border-2 text-gray-300 rounded-lg border-gray-300 float-right" @click="showForm">Order Now!</button>
            </div>
        </div>
        <div class="-mb-20 sm:mb-0">
            <img class="m-auto sm:hidden" :src="imageSmall" alt="Burger Image">
            <img class="m-auto hidden sm:block" :src="imageBig" alt="Burger Image">
        </div>
    </div>
</template>