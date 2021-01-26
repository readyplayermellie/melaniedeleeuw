<template>
  <div id="app">
    <Navbar />
    <Header />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Header,
    Footer
  }
}
</script>

<style>
body {
  background-color: #1D1135;
}
</style>
