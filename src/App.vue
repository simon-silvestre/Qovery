<template>
  <div id="app">
    <Header />
    <Work />
    <Usage />
    <Features />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Work from './components/Work.vue'
import Usage from './components/Usage.vue'
import Features from './components/Features.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Work,
    Usage,
    Features,
    Footer
  }
}
</script>

<style lang="scss">
  * {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  #app {
    font-family: 'Questrial', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    background-color: #F9F9FD;
    image-rendering: -webkit-optimize-contrast;
  }
</style>
