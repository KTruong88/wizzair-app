<template>
  <div id="app">
    <Navbar />
    <Jumbotron />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Jumbotron from './components/jumbotron'

export default {
  name: 'App',
  components: {
    Navbar,
    Jumbotron
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
