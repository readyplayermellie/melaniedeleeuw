<template>
  <div id="app">
    <Navbar />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@100;300;400&display=swap');

#app {
  background-color: #1D1135;
  font-family: 'Lato', sans-serif;
  font-weight: 300;
  color: #FCFBFE;
  height: 100vh;
}

h1,
h2 {
  margin: 0;
  font-family: 'Lato', sans-serif;
  font-weight: 100;
  color: #FCFBFE;
  text-transform: uppercase;
  letter-spacing: 5px;
}

p {
  margin: 0;
}

a {
  text-decoration: none;
  color: #FCFBFE;
  margin: 0;
}

ul {
  list-style: none;
  margin: 0;
}

.btn {
  border-radius: 50px;
  text-transform: uppercase;
  font-family: 'Lato', sans-serif;
  color: #FCFBFE;
  font-weight: 300;
  width: 260px;
  padding: 10px;
  letter-spacing: 3px;
}