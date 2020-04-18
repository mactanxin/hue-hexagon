<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <hexagon></hexagon>
    <hexagon></hexagon>
    <hexagon></hexagon>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Hexagon from './components/Hexagon.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Hexagon
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
