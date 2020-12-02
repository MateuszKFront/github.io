<template>
  <div id="app">
    <homepage/>
  </div>
</template>

<script>
import homepage from './components/home.vue'

export default {
  name: 'App',
  components: {
    homepage
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
body{
  margin:0px;
  padding: 0px;
}
</style>
