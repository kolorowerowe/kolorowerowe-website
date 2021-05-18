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
html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  overflow: overlay;
}

body, button {
  font-family: "Montserrat", sans-serif;
}

.white-btn {
  padding: 15px;
  border: 2px solid #fff;
  border-radius: 0;
  color: white;
  background-color: transparent;
  font-size: 20px;
  transition: background-color 200ms linear, border-color 200ms linear;
}

.white-btn:hover {
  background-color: #e43f5a;
  border-color: #e43f5a;
}


body::-webkit-scrollbar {
  width: 6px;
  background-color: transparent;
}

body::-webkit-scrollbar-thumb {
  border-radius: 5px;
  background: linear-gradient(80deg, #1f4068, #1b1b2f, #e43f5a);
  background-size: 400% 400%;
}

</style>
