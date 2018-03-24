<template>
  <div>
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                :interval="4000"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >
      <b-carousel-slide
                        class="slide1"
      ></b-carousel-slide>

      <b-carousel-slide
                        class ="slide2"
      ></b-carousel-slide>

      <b-carousel-slide
                        class ="slide3"
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

.slide1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/shutterstock_273033479_4d42c0fe.jpg");
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 475px;
}
.slide2 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/rix_721ed023.jpg");
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 475px;
}
.slide3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/plq_f0413d49.jpg");
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 475px;
}
</style>
