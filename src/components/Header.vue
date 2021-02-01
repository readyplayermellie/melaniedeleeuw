<template>
  <div id="header-container">
    <div id="pink-moon" />
    <div id="header-box">
      <h1>{{ title }}</h1>
      <h2>{{ subtitle }}</h2>
      <button class="btn btn-primary">Do something</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      title: 'Melanie de Leeuw',
      subtitle: 'A frontend portfolio',
    }
  }

}
</script>

<style scoped>
#header-container {
  text-align: center;
  padding-top: 90px;
  height: 400px;
  width: 100%;
}
h1 {
  font-size: 56px;
}
h1, h2, button {
  margin-bottom: 25px;
}

button {
  margin-top: 45px;
}

#pink-moon {
  width: 450px;
  height: 400px;
  border-radius: 50%;
  -webkit-box-shadow: 0px -7px 20px 6px rgba(186,30,104,0.89);
  -moz-box-shadow: 0px -7px 20px 6px rgba(186,30,104,0.89);
  box-shadow: 0px -7px 20px 6px rgba(186,30,104,0.89);
  margin: auto;
}

#header-box {
  padding: 20px;
  background-color: #1D1135;
  margin-top: -220px;
}

</style>
