<template>
  <div id="app">
    <Navbar />
    <router-view class="view"/>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@100;300;400&display=swap');

* {
  margin: 0;
  padding: 0;
  border: 0;
}
body {
  background-color: #000619;
  font-family: 'Lato', sans-serif;
  font-weight: 300;
  color: #FCFBFE;
}

.view {
  max-width: 980px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 8%;
  margin-bottom: 8%;
}
h1  { 
  font-size: 2.6em;
  text-align: center;
} 
     
h2 { 
  font-size: 2.0em;
} 
    
p { 
  font-size: 1.2em;
  font-weight: 300;
  letter-spacing: 3px;
}

h1,
h2,
h3 {
  font-weight: 300;
  text-transform: uppercase;
  letter-spacing: 5px;
}
a {
  text-decoration: none;
  color: #FCFBFE;
}

</style>