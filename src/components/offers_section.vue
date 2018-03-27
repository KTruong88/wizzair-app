<template>
  <div class="wrapper">
    <h1 class="title-wrap">
      <p class="title">Hand pick the offers you like best</p>
    </h1>

    <div class="banner-wrap">

      <div class="top-left-wrapper">
        <div class="banner banner1">

        </div>

        <div class="banner2">
          <p class="banner2-title">
            Booking.com
          </p>
          <p class="banner2-content">
            Book today and get <strong>10% of your hotel booking back!</strong>
          </p>
        </div>
      </div>

      <div class="top-right-wrapper">
        <div class="banner banner3">

        </div>

        <div class="banner4">
          <p class="banner4-title">
            Car Rental
          </p>
          <p class="banner4-content">
            Enjoy <strong>7% Wizz Air credit</strong>
            when you book your car rental
          </p>
        </div>
      </div>


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
  flex-direction: column;
  width: 100%;
  height: 600px;
  background-color: #f2f2f2;
  padding: 0 20px;
  margin: 0 auto;
}

.title-wrap {
  display: flex;
  max-width: 1400px;
  width: 100%;
  padding: 0 20px;
  margin: 0 auto;
}

.title {
  width: 100%;
  height: 40px;
  font-size: 24px;
  font-weight: 300;
  margin-top: -10px;
  color: #06038d;
  text-align: left;
}

.banner-wrap {
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding-left: 20px;
}

.top-left-wrapper, .top-right-wrapper {
  display: flex;
  width: 100%;
  margin-right: 20px;
}

.banner {
  height: 140px;
  width: 100%;
  max-width: 331px;
  background-size: cover;
}
.banner1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/booking_com_ccd40dc0.jpg");
}

.banner3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/car-rental_c9015673.jpg");
}

.banner2, .banner4 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  height: 140px;
  width: 338px;
  background-color: #fff;
}

.banner2-title, .banner4-title {
  display: block;
  padding: 0 30px 5px 0;
  margin: 0;
  font-size: 16px;
  font-weight: 700;
  color: #c6007e;
  text-transform: uppercase;
  margin-left: 15px;
  margin-top: 15px;
}

.banner2-content, .banner4-content{
  margin-top: 0;
  margin-bottom: 2rem;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  font-size: 14px;
  font-weight: 400;
  text-align: left;
  margin-left: 15px;
}

strong {
  color: #c6007e;
}
</style>
