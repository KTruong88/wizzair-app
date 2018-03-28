<template>
  <div>
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                :interval="4000"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >
      <b-carousel-slide class="slide1">
        <div class="hero-banner-wrap">
          <div class="hero-banner">
            <img src="https://wizzair.com/static/docs/default-source/promotions/winter-schedule-2018/promo_en_15d178a7.svg"
            >
          </div>
        </div>
      </b-carousel-slide>

      <b-carousel-slide class ="slide2">
        <div class="hero-banner-wrap2">
          <div class="hero-banner2">
            <h2 class="hero-banner-title">
              <div class="title">from Podgorica**
                  <h1 class="title-text">Milan</h1>
              </div>
              <strong class="hero-banner__price">‎​€​9.99</strong>
            </h2>
          </div>
        </div>
      </b-carousel-slide>

      <b-carousel-slide class ="slide3">
        <div class="hero-banner-wrap2">
          <div class="hero-banner2">
            <h2 class="hero-banner-title">
              <div class="title">from Glasgow **
                  <h1 class="title-text">Katowice</h1>
              </div>
              <strong class="hero-banner__price">‎​£​22.99</strong>
            </h2>
          </div>
        </div>
      </b-carousel-slide>

<!-- Carousel form -->

  <div class="carousel-form">

    <div class="side-buttons">
      <button class="buttons button1">
        <icon name=""></icon>
        <icon name="fighter-jet"></icon> <br>
        Flights
      </button>
      <button class="buttons">

        <icon
                    name="fighter-jet"
                   class="fighter-jet-icon"
                   style="height: 1.2rem;
                          margin-left: 20px;
                          margin-bottom: -16px;
                          background-color: #6495ED;
                          padding: 2px;
                          border-radius: 3px;"
          >
        </icon>
        <br>

        <icon
                    name="plus"
                   class="plus-icon"
                   style="height: .8rem;
                          margin-top: -20px;
                          margin-bottom: -5px;
                          background-color: #6495ED;
                          padding: 2px;
                          border-radius: 3px;"
          >
        </icon>
         <br>

        <icon       name="bed"
                   class="bed-icon"
                   style="height: 1.2rem;
                          margin-right: 20px;
                          margin-top: -10px;
                          background-color: #6495ED;
                          padding: 2px;
                          border-radius: 3px;"
          >
        </icon>
         <br>
        <p class="flight-txt">Flight & Hotel</p>
      </button>
      <button class="buttons">
        <icon name="hotel"></icon> <br>
        Hotels
      </button>
      <button class="buttons button4">
        <icon name="automobile"></icon> <br>
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

        <div class="input-wrap">
          <input type="text" class="input-half input-left" placeholder="DEPARTURE">

          <div class="right-arrow">

          </div>
          <input type="text" class="input-half input-right" placeholder="RETURN">
        </div>
        <b-form-input class="input input4" placeholder="PASSENGERS">

        </b-form-input>
        <button class="submit-button">
          Search
        </button>

        <div class="links-container">
          <a href="" class="dates-link">Flexible on Dates?</a>
          <a href="" class="search-link"> New Search</a>
        </div>

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

.fa-icon {
  width: auto;
  height: 2.3em; /* or any other relative font sizes */
  color: darkblue;

  /* You would have to include the following two lines to make this work in Safari */
  max-width: 100%;
  max-height: 100%;
}

.slide1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/shutterstock_273033479_4d42c0fe.jpg");
  background-size: cover;
  background-position: center;
  z-index: 0;
  width: 100%;
  height: 475px;
}

.hero-banner-wrap {
  width: 56%;
  height: 243px;
  margin-left: 61%;
}

.hero-banner {
  height: 100%;
  width: 100%;
  background-color: rgba(198,0,126,.9);
  padding: 20px 20px 10px;
}

.hero-banner-title {
  display: flex;
  justify-content: space-between;
}

.title {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  font-size: 13px;
  font-weight: 400;
  text-align: left;
}

.title-text {
  font-family: P22 Underground Pro,sans-serif;
  font-size: 40px;
  font-weight: 300;
}

.hero-banner__price {
  font-family: P22 Underground Pro,sans-serif;
  font-size: 40px;
  font-weight: 300;
}

.hero-banner-wrap2 {
  width: 57%;
  height: 118px;
  margin-left: 61%;
}

.hero-banner2 {
  height: 100%;
  width: 100%;
  background-color: rgba(198,0,126,.9);
  padding: 20px 20px 10px;
}

.hero-banner:hover {
  cursor: pointer;
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
  width: 29.3%;
  height: 423px;
}

.side-buttons {
  display: flex;
  flex-direction: column;
  width: 100px;
}

.buttons {
  height: 106px;
  background-color: #E8E8E8;
  font-size: 12px;
  color: #919191;
  text-align: center;
  word-break: break-word;
  overflow-wrap: break-word;
  font-weight: 700;
  text-transform: uppercase;
}

.buttons:hover {
  cursor: pointer;
  background-color: #fff;
}

.buttons:focus {
  box-shadow: 0 2px 3px rgba(0,0,0,.2);
  background-color: #f2f2f2;
  color: #06038d;
}

.button1 {
  border-top-left-radius: 5px;
}

.button4 {
  border-bottom-left-radius: 5px;
}

.links-container {
  margin-bottom: -15px;
}

.dates-link {
  float: left;
  font-size: 11px;
  font-weight: 700;
  color: #a6006a;
  text-decoration: underline;
  text-transform: uppercase;
  text-shadow: none;
}

.search-link {
  float: right;
  font-size: 11px;
  font-weight: 700;
  color: #a6006a;
  text-decoration: underline;
  text-transform: uppercase;
  text-shadow: none;
}

.flight-txt {
  font-size: 11px;
}

@media only screen and (max-width:810px) {
  .carousel-form {
    flex-direction: column;
  }
  .buttons {
    height: 55px;
    width: 25%;
  }
  .buttons:focus {
    box-shadow: 1px 0px 0px;
  }
  .side-buttons {
    width: 100%;
    flex-direction: row;
  }
  .input-half, .input4 {
    display: none;
  }
  .input2 {
    margin-bottom: -90px;
  }
  .bottom-wrapper {
    display: none;
  }
  .hero-banner-wrap {
    display: none;
  }
  .right-arrow {
    display: none;
  }
  .hero-banner-wrap2 {
    display: none;
  }
  .carousel-form {
    width: 90% !important;
    height: 320px !important;
  }
  .submit-button {
    margin-top: 15px;
  }
  .dates-link {
    margin-top: -40px;
  }
  .search-link {
    margin-top: -40px;
  }
  .fa-icon {
    margin-bottom: -5px;
    width: auto;
    height: 1.3em; /* or any other relative font sizes */

    /* You would have to include the following two lines to make this work in Safari */
    max-width: 100%;
    max-height: 100%;
  }
  .fighter-jet-icon {
    margin-left: 50px !important;
    margin-bottom: -4px !important;
  }
  .plus-icon {
    margin-bottom: 4px !important;
  }
  .bed-icon {
    margin-right: 125px !important;
    margin-bottom: 20px !important;
  }
  .flight-txt {
    margin-top: -45px !important;
  }

}

@media only screen and ( max-width:1100px) {
  .carousel-form {
    z-index: 1000;
    position: absolute;
    margin-top: -450px;
    margin-left: 40px;
    border-radius: 5px;
    background-color: #f2f2f2;
    box-shadow: 1px 0 2px rgba(0,0,0,.2);
    width: 40%;
    height: 423px;
  }
  .hero-banner2 {
    width: 100%;
    min-width: 340px;
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

.input-wrap {
  display: flex;
  width: 100%;
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

.input::placeholder {
  color: #C0C0C0;
}

.input1 {
  border-bottom-right-radius: 0px;
  border-bottom-left-radius: 0px;
  border-bottom: transparent;
}

.input1:focus {
  border-bottom: none !important;
}

.form-control:focus {
  outline: 0;
  z-index: 20;
  border: 2px solid #919191;
  -webkit-box-shadow: 6px 11px 21px -1px rgba(145,145,145,0.56);
  -moz-box-shadow: 6px 11px 21px -1px rgba(145,145,145,0.56);
  box-shadow: 6px 11px 21px -1px rgba(145,145,145,0.56);
}

.input2 {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}

.input2:focus {
  border-top: 1px solid #919191;
}

.input-half {
  width: 100%;
  height: 62px;
  font-size: 16px;
  color: #343434;
  border: 1px solid #919191;
  padding-bottom: 20px;
  margin-top: -5px;
}

.input-left {
  border-top-left-radius: 3px;
  border-bottom-left-radius: 3px;
  border-right: transparent;
  color: transparent;
}

.input-left::placeholder {
  font-size: 11px;
  font-weight: bold;
  text-indent: 15px;
}

.input-left:hover {
  cursor: pointer;
  outline: none;
}

.input-left:focus {
  border-top: 2px solid #919191;
  border-left: 2px solid #919191;
  border-bottom: 2px solid #919191;
}

.input-right {
  border-top-right-radius: 3px;
  border-bottom-right-radius: 3px;
}

.input-right:hover {
  cursor: pointer;
}

.input-right::placeholder {
  font-size: 11px;
  font-weight: bold;
  text-indent: 15px;
}

.input-right:focus {
  border-top: 2px solid #919191;
  border-right: 2px solid #919191;
  border-bottom: 2px solid #919191;
  color: transparent;
}

.input4 {
  padding-bottom: 30px;
  color: transparent;
}

.input4:hover {
  cursor: pointer;
}

.input4::placeholder {
  color: #919191;
  font-size: 11px;
  font-weight: bold;
}

textarea:hover,
input:hover,
textarea:active,
input:active,
textarea:focus,
input:focus,
button:focus,
button:active,
button:hover,
label:focus,
.btn:active,
.btn.active {
    outline:0px !important;
    -webkit-appearance:none;
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

.right-arrow {
	position: relative;
	background: #fff;
}
.right-arrow:after, .right-arrow:before {
	left: 100%;
	top: 50%;
	border: solid transparent;
	content: " ";
	height: 0;
	width: 0;
	position: absolute;
	pointer-events: none;
}

.right-arrow:after {
	border-color: rgba(255, 255, 255, 0);
	border-left-color: #fff;
	border-width: 8px;
	margin-top: -8px;
}

.right-arrow:before {
	border-color: rgba(145, 145, 145, 0);
	border-left-color: #919191;
	border-width: 9px;
	margin-top: -9px;
}

</style>
