<template lang="pug">
  div#app
    img(src="./assets/logo.png")
    router-view
    el-time-select(v-model="value1", :picker-options="{start: '08:30', step: '00:15', end: '18:30'}", placeholder="Select time")
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      value1: ''
    }
  }
}
</script>

<style lang="sass">
#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50
  margin-top: 60px
</style>
