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

    export default {
        data() {
            return {
                sectionHeader: 'Menu',
                products: [
                    { name: 'Sample Burger 1', image: product1, price: 56.97 },
                    { name: 'Sample Burger 2', image: product2, price: 62.56 },
                    { name: 'Sample Burger 3', image: product3, price: 67.09 },
                    { name: 'Sample Burger 4', image: product4, price: 55.70 },
                    { name: 'Sample Burger 5', image: product5, price: 68.74 },
                    { name: 'Sample Burger 6', image: product6, price: 81.18 },
                    { name: 'Sample Burger 7', image: product7, price: 88.70 },
                    { name: 'Sample Burger 8', image: product8, price: 57.49 },
                    { name: 'Sample Burger 9', image: product9, price: 76.62 },
                    { name: 'Sample Burger 10', image: product10, price: 66.05 },
                ]
            }
        }
    }
</script>

<template>
    <div class="py-6" id="menu"></div>
    <div class="px-4 pb-16 flex flex-col gap-12 sm:max-w-7xl sm:m-auto">
        <h2 class="text-4xl text-yellow-400 font-bold">{{ sectionHeader }}</h2>
        <div class="flex flex-col gap-3">
            <div v-for="product in products">
                <div class="flex flex-row items-center sm:gap-4">
                    <p class="text-lg text-gray-100 float-left">{{ product['name'] }}</p>
                    <div class="mx-1 h-3 block relative float-left border-b-2 border-yellow-400 border-dotted w-full"></div>
                    <p class="text-lg text-gray-100 float-left">${{ product['price'] }}</p>
                </div>
            </div>
        </div>
    </div>
</template>