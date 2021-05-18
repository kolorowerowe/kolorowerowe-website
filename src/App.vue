<template>
  <div id="app">
    <Hello/>
    <AppBar/>
  </div>
</template>

<script>
import Hello from './components/Hello.vue'
import AppBar from './components/AppBar.vue'


export default {
  name: 'App',
  components: {
    Hello,
    AppBar
  }
}
</script>

<style>

body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
  padding: 0
}
</style>
