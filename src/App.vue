<script>
  import Header from './components/Header.vue'
  import Hero from './components/Hero.vue'
  import AboutUs from './components/AboutUs.vue'
  import Products from './components/Products.vue'
  import Menu from './components/Menu.vue'
  import Procedure from './components/Procedure.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: { Header, 
      Hero, 
      AboutUs, 
      Products, 
      Menu, 
      Procedure,
      Footer },
    data() {
      return {
        text: 'Sample Text'
      }
    }
  }
</script>

<template>
  <div class="sm:relative sm:pb-20 sm:h-full">
    <Hero />
    <Header />
  </div>
  <AboutUs />
  <Products />
  <Menu />
  <Procedure />
  <Footer />
</template>
