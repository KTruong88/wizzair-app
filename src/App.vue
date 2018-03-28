<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <SearchTools />
    <CheapFlight />
    <OffersTop />
    <OffersBottom />
    <Opportunity />
    <ContactSocials />
    <ExternalFooter />
    <SitemapFooter />
    <DisclaimerFooter />
  </div>
</template>

<script>
import Navbar from './components/navbar'
import Carousel from './components/carousel'
import SearchTools from './components/search_tools'
import CheapFlight from './components/cheap_flight'
import OffersTop from './components/offers_section_top'
import OffersBottom from './components/offers_section_bottom'
import Opportunity from './components/opportunity'
import ContactSocials from './components/contact_socials'
import ExternalFooter from './components/external_footer'
import SitemapFooter from './components/sitemap_footer'
import DisclaimerFooter from './components/disclaimer_footer'

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    SearchTools,
    CheapFlight,
    OffersTop,
    OffersBottom,
    Opportunity,
    ContactSocials,
    ExternalFooter,
    SitemapFooter,
    DisclaimerFooter,
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
