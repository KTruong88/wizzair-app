<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <SearchTools />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Carousel from './components/carousel'
import SearchTools from './components/search_tools'

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    SearchTools,
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
