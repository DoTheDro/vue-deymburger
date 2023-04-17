<script>
    import procedure1 from '../assets/images/procedure-1.png'
    import procedure2 from '../assets/images/procedure-2.png'
    import procedure3 from '../assets/images/procedure-3.png'
    import procedure4 from '../assets/images/procedure-4.png'

    export default {
        data() {
            return {
                procedure1: procedure1,
                procedure2: procedure2,
                procedure3: procedure3,
                procedure4: procedure4,
                sectionHeader: 'Procedure'
            }
        }
    }
</script>

<template>
    <div class="py-6" id="procedure"></div>
    <div data-aos="flip-down" 
        data-aos-duration="800"
        data-aos-once="true"
    class="px-4 pb-16 flex flex-col gap-12 sm:max-w-7xl sm:m-auto">
        <h2 class="text-4xl text-yellow-400 font-bold">{{ sectionHeader }}</h2>
        <div class="flex flex-col gap-6">
            <div data-aos="flip-down" 
                data-aos-duration="1000"
                data-aos-once="true" 
                class="p-4 bg-yellow-400 rounded-lg flex flex-row gap-6 items-center max-w-xl m-auto md:ml-40">
                <div class="custom-max-width">
                    <img :src="procedure1" alt="Procedure 1">
                </div>
                <div>
                    <p class="text-base sm:text-lg">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus, beatae!</p>
                </div>
            </div>
            
            <div data-aos="flip-down" 
                data-aos-duration="1300"
                data-aos-once="true"  
                class="p-4 bg-yellow-400 rounded-lg flex flex-row-reverse gap-6 items-center max-w-xl m-auto md:mr-40">
                <div class="custom-max-width">
                    <img :src="procedure2" alt="Procedure 2">
                </div>
                <div>
                    <p class="text-base sm:text-lg">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus, beatae!</p>
                </div>
            </div>
            
            <div data-aos="flip-down" 
                data-aos-duration="1600"
                data-aos-once="true"  
                class="p-4 bg-yellow-400 rounded-lg flex flex-row gap-6 items-center max-w-xl m-auto md:ml-40">
                <div class="custom-max-width">
                    <img :src="procedure3" alt="Procedure 3">
                </div>
                <div>
                    <p class="text-base sm:text-lg">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus, beatae!</p>
                </div>
            </div>
            
            <div data-aos="flip-down" 
                data-aos-duration="1900"
                data-aos-once="true"  
                class="p-4 bg-yellow-400 rounded-lg flex flex-row-reverse gap-6 items-center max-w-xl m-auto md:mr-40">
                <div class="custom-max-width">
                    <img :src="procedure4" alt="Procedure 4">
                </div>
                <div>
                    <p class="text-base sm:text-lg">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ducimus, beatae!</p>
                </div>
            </div>
        </div>
    </div>
</template>