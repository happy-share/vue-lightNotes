<template>
  <div id="app">
    <img src="../assets/logo.png">
  </div>
</template>

<script>
export default {
  name: 'demo',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    startHacking () {
      this.$toast('It Works!')
    }
  }
}
</script>

<style>

</style>
