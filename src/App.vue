<template>
  <div id="app">
    <card-input-demo></card-input-demo>
  </div>
</template>

<script>
import CardInputDemo from './components/CardInputDemo.vue'

export default {
  name: 'App',
  components: {
    CardInputDemo
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
