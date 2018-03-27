<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <SearchTools />
    <CheapFlight />
    <Offers />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Carousel from './components/carousel'
import SearchTools from './components/search_tools'
import CheapFlight from './components/cheap_flight'
import Offers from './components/offers_section'

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    SearchTools,
    CheapFlight,
    Offers,
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
