<template>
  <div id="app">
    <master/>
  </div>
</template>

<script>
import Master from './components/Master.vue'

export default {
  name: 'app',
  components: { Master }
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #00a81c;
    margin-top: 10px;
    background: #282c25;
  }
</style>
