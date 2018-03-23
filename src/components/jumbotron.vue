<template>
  <div>
    <b-carousel id="carousel1"
                background="#ababab"
                :interval="4000"
                img-width="100%"
                img-height="auto"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >
      <b-carousel-slide media="(min-width:1441px)"
                        img-src="https://wizzair.com/static/images/default-source/banner-images/shutterstock_273033479_4d42c0fe.jpg"
      ></b-carousel-slide>

      <b-carousel-slide media="(min-width:1441px)"
                        img-src="https://wizzair.com/static/images/default-source/banner-images/rix_721ed023.jpg"
      ></b-carousel-slide>

      <b-carousel-slide media="(min-width:1441px)"
                        img-src="https://wizzair.com/static/images/default-source/banner-images/plq_f0413d49.jpg"
      ></b-carousel-slide>
    </b-carousel>

  </div>
</template>

<script>
export default {
  data () {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
<style scoped>
.carousel-control-next-icon {
  display: none !important;
}
</style>
