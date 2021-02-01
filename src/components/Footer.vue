<template>
  <div id="footer-container">
    <button class="btn btn-secondary" :onclick="url">{{ btnSend }}</button>
    <pre>{{ copyright }}</pre>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      url: "location.href='mailto:melaniedeleeuw@gmail.com'",
      btnSend: 'Send me an email',
      copyright: 'Copyright 2021, Mellie',
    }
  }
}
</script>

<style scoped>
#footer-container {
  text-align: center;
  width: 100%;
  position: fixed;
  left: 0;
  bottom: 0;
}
</style>