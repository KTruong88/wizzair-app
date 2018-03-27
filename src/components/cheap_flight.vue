<template>
  <div class="wrapper">
    <h1 class="title">
      Cheap flight offers**
    </h1>

    <div>
        <b-carousel id="carousel1"
                    controls
                    indicators
                    background="#fff"
                    :interval="0"
                    v-model="slide"
                    @sliding-start="onSlideStart"
                    @sliding-end="onSlideEnd"
        >

          <b-carousel-slide
                        class="cards card1"
          >
            <div class="card-text-wrapper">
              <div class="card-content-wrapper">
                <p class="card-title">Budapest</p>

                <p class="card-content">
                  from Baku**
                </p>
              </div>

            </div>
          </b-carousel-slide>

          <b-carousel-slide
                        class="cards card2"
          >

          </b-carousel-slide>

          <b-carousel-slide
                        class="cards card3"
          >

          </b-carousel-slide>

          <b-carousel-slide
                        class="cards card4"
          >

          </b-carousel-slide>

        </b-carousel>
      </div>
  </div>
</template>

<script>
export default {
}


</script>

<style scoped>

.wrapper {
  display: flex;
  width: 100%;
  flex-direction: column;
  max-width: 1400px;
  padding: 0 20px;
  margin: 0 auto;
  background-color: #f2f2f2;
}

.title {
  margin-top: 20px;
  font-size: 24px;
  font-weight: 300;
  color: #06038d;
  align-self: flex-start;
  margin-bottom: 30px;
}

.cards {
  max-width: 442px;
  width: 442;
  height: 250px;
  background-repeat: no-repeat;
  background-size: cover;
}
.card1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/bud_1_6f5475bf.jpg");
}

.card2 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/tsr_5d6c8fbf.jpg");
}
.card3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/waw_7ef0c47c.jpg");
}
.card4 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/plq_0f0e3515.jpg");
}

.card-text-wrapper {
  display: flex;
  flex-direction: column;
}

.card-title-wrapper {
  padding: 0 10px 0 20px;
  font-weight: 700;
  font-family: P22 Underground Pro,sans-serif;
  font-size: 16px;
  color: #c6007e;
  text-transform: uppercase;
  width: 442px;
}

.card-title {
  margin-top: 10px;
  font-family: P22 Underground Pro,sans-serif;
  font-weight: 700;
  text-shadow: none;
  font-size: 16px;
  color: #c6007e;
  text-transform: uppercase;
  margin-bottom: 0px;
}

.card-content-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0 10px 0 20px;
  vertical-align: middle;
  background-color: #fff;
  width: 442px;
  height: 100px;
  margin-bottom: -40px;
  margin-left: -66px;
}

.card-content {
  font-size: 14px;
  color: #000;
  text-shadow: none;
}


</style>
