<template>
  <div id="app">
    <Navbar />
    <Carousel />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Carousel from './components/carousel'

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
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
