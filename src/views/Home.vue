<template>
    <TypeTitle :title="title"/>
</template>

<script>
import TypeTitle from '../components/TypeTitle'

export default {
  name: 'Home',
  components: {
    TypeTitle,
  },
  data() {
    return {
      title: '[Welcome to Ready Player Mellie]',
    }
  }
}
</script>
