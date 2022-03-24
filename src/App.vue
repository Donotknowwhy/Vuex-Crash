<template>
  <div id="app">
      <Navbar />
    <Todos />
    <StatusBar />
    <ProgressBar />
  </div>
</template>

<script>
import ProgressBar from './components/ProgressBar.vue'
import StatusBar from './components/StatusBar.vue'
import Navbar from './components/Navbar.vue'
import Todos from './components/Todos.vue'

export default {
  name: 'App',
  components: {
   Todos, Navbar, StatusBar, ProgressBar
  }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: rgb(219, 219, 219);
  margin: 20px auto;
  width: 90%;
  max-width: 800px;
}
</style>
