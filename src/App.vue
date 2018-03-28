<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <SearchTools />
    <CheapFlight />
    <OffersTop />
    <OffersBottom />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Carousel from './components/carousel'
import SearchTools from './components/search_tools'
import CheapFlight from './components/cheap_flight'
import OffersTop from './components/offers_section_top'
import OffersBottom from './components/offers_section_bottom'

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    SearchTools,
    CheapFlight,
    OffersTop,
    OffersBottom,
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
