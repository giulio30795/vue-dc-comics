<template>
  <div id="app">
    <Header />
    <Hero />
    <Content />
    <Footer />
  </div>
</template>

<script>

import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import Footer from '@/components/Footer.vue'
import Hero from '@/components/Hero.vue'
  

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Footer,
    Hero,
  }

}
</script>

<style lang="scss">

</style>
