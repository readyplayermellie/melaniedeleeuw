<template>
  <div id="card">
    <h3> {{ title }} </h3>
    <p>{{ content }}</p>
    <a href="#">{{ linkText }}</a>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    content: String,
    linkText: String,
  },
}
</script>

<style scoped>
#card {
  padding: 5px;
  height: 300px;
  width: 250px;
  border: 1px solid #BA1E68;
  border-radius: 20px;
  -webkit-box-shadow: 0px 2px 5px 2px rgba(186,30,104,1);
  -moz-box-shadow: 0px 2px 5px 2px rgba(186,30,104,1);
  box-shadow: 0px 2px 5px 2px rgba(186,30,104,1);
}

h3 {
  text-align: center;
  padding: 25px;
}
</style>