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

<!-- Carousel form -->

  <div class="carousel-form">

    <div class="side-buttons">
      <button class="buttons">
        Flights
      </button>
      <button class="buttons">
        Flight & Hotel
      </button>
      <button class="buttons">
        Hotels
      </button>
      <button class="buttons">
        Cars
      </button>
    </div>

    <b-form class="bform">
      <div class="top-wrapper">
        <b-form-input class="input input1" type="text" placeholder="Origin">
        </b-form-input>

        <div class="arrow_box">

        </div>

        <b-form-input class="input input2" type="text" placeholder="Destination">
        </b-form-input>

      </div>

      <div class="top-wrapper bottom-wrapper">

        <b-form-input class="input input3">

        </b-form-input>
        <b-form-input class="input input4">

        </b-form-input>
        <button class="submit-button">
          Search
        </button>
      </div>
    </b-form>
  </div>
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
  z-index: 0;
  width: 100%;
  height: 475px;
}
.slide2 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/rix_721ed023.jpg");
  background-size: cover;
  background-position: center;
  z-index: 0;
  width: 100%;
  height: 475px;
}
.slide3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/plq_f0413d49.jpg");
  background-size: cover;
  background-position: center;
  z-index: 0;
  width: 100%;
  height: 475px;
}

.carousel-form {
  display: flex;
  z-index: 100;
  position: absolute;
  margin-top: -450px;
  margin-left: 40px;
  border-radius: 5px;
  background-color: #f2f2f2;
  box-shadow: 1px 0 2px rgba(0,0,0,.2);
  width: 28%;
  height: 425px;
}

.side-buttons {
  display: flex;
  flex-direction: column;
  border: 1px solid red;
  width: 80px;
}

.buttons {
  height: 106px;
}
@media only screen and (max-width:1100px) {
  .carousel-form {
    z-index: 1000;
    position: absolute;
    margin-top: -450px;
    margin-left: 40px;
    border-radius: 5px;
    background-color: #f2f2f2;
    box-shadow: 1px 0 2px rgba(0,0,0,.2);
    width: 40%;
    height: 420px;
  }
}

.bform {
  display: flex;
  flex-direction: column;
  width: 100%;
}
.top-wrapper {
  display: flex;
  align-self: center;
  margin-top: 20px;
  flex-direction: column;
  justify-content: center;
  width: 88%;
  height: 138px;
}

.bottom-wrapper {
  justify-content: space-between;
  height: 220px;
}

.submit-button {
  color: #fff;
  text-align: center;
  border-radius: 3px;
  background-color: #c6007e;
  text-transform: uppercase;
  font-family: P22 Underground Pro,sans-serif;
  height: auto;
  font-weight: 450;
  cursor: pointer;
  vertical-align: middle;
  min-width: 150px;
  padding: 15px 20px;
  font-size: 14px;
}

.input {
  width: 100%;
  height: 70px;
  font-size: 22px;
  font-weight: 400;
  font-family: Source Sans Pro,sans-serif;
  border-top-right-radius: 3px;
  border-top-left-radius: 3px;
  border: 1px solid #919191;
}

.input1 {
  border-bottom-right-radius: 0px;
  border-bottom-left-radius: 0px;
  border-bottom: transparent;
}

.input2 {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}

.arrow_box {
	position: relative;
	background: #fff;
}

.arrow_box:after, .arrow_box:before {
	top: 100%;
	left: 50%;
	border: solid transparent;
	content: " ";
	height: 0;
	width: 0;
	position: absolute;
	pointer-events: none;
}

.arrow_box:after {
	border-color: rgba(255, 255, 255, 0);
	border-top-color: #fff;
	border-width: 8px;
	margin-left: -8px;
}

.arrow_box:before {
	border-color: rgba(145, 145, 145, 0);
	border-top-color: #919191;
	border-width: 9px;
	margin-left: -9px;
}
</style>
