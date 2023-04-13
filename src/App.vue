<script>
  import Header from './components/Header.vue'
  import Hero from './components/Hero.vue'
  import AboutUs from './components/AboutUs.vue'

  export default {
    components: { Header, Hero, AboutUs },
    data() {
      return {
        text: 'Sample Text'
      }
    }
  }
</script>

<template>
  <div>
    <Hero />
    <Header />
  </div>
  <AboutUs />
</template>
