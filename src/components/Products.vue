<script>
    import product1 from '../assets/images/product-1.png'
    import product2 from '../assets/images/product-2.png'
    import product3 from '../assets/images/product-3.png'
    import product4 from '../assets/images/product-4.png'
    import product5 from '../assets/images/product-5.png'
    import product6 from '../assets/images/product-6.png'
    import product7 from '../assets/images/product-7.png'
    import product8 from '../assets/images/product-8.png'
    import product9 from '../assets/images/product-9.png'
    import product10 from '../assets/images/product-10.png'

    //Slider Imports
    import { Swiper, SwiperSlide } from 'swiper/vue'
    import 'swiper/css'
    import 'swiper/css/pagination'
    import { Pagination } from 'swiper'


    export default {
        components: {
            Swiper,
            SwiperSlide
        },
        setup() {
            return {
                modules: [Pagination]
            }
        },
        data() {
            return {
                products: [
                    { name: 'Sample Burger 1', image: product1, price: 56 },
                    { name: 'Sample Burger 2', image: product2, price: 62 },
                    { name: 'Sample Burger 3', image: product3, price: 67 },
                    { name: 'Sample Burger 4', image: product4, price: 55 },
                    { name: 'Sample Burger 5', image: product5, price: 68 },
                    { name: 'Sample Burger 6', image: product6, price: 81 },
                    { name: 'Sample Burger 7', image: product7, price: 88 },
                    { name: 'Sample Burger 8', image: product8, price: 57 },
                    { name: 'Sample Burger 9', image: product9, price: 76 },
                    { name: 'Sample Burger 10', image: product10, price: 66 },
                ]
            }
        }
    }
</script>

<template>
    <div class="px-5 pb-16">
        <h2 class="text-4xl text-yellow-400 font-bold">Our Products</h2>
        <div class="">
            <swiper
                class="my-swiper"
                :slidesPerView="3"
                :spaceBetween="0"
                :centeredSlides="true"
                :pagination="{
                    clickable: true,
                }"
                :modules="modules"
                :breakpoints="{
                    '200': {
                        slidesPerView: 1,
                    },
                    '640': {
                        slidesPerView: 2,
                        spaceBetween: 25
                    },
                    '758': {
                        slidesPerView: 3
                    },
                }"
            >
                <swiper-slide class="" v-for="(product, key) in products">
                    <div class="bg-gray-700 px-4 py-5 rounded-xl max-w-sm m-auto">
                        <div class="max-w-xs w-full">
                            <img :src="product['image']" alt="">
                        </div>
                        <h2 class="text-2xl text-gray-200">{{ product['name'] }}</h2>
                        <p class="text-2xl text-gray-200">{{ product['price'] }}</p>
                        <p class="text-2xl text-gray-200">{{ key }}</p>
                    </div>
                </swiper-slide>
            </swiper>
        </div>
    </div>
</template>