<template>
  <div class="wrapper">
    <h1 class="title-wrap">
      <p class="title">Hand pick the offers you like best</p>
    </h1>

    <div class="banner-wrap">

      <div class="top-left-wrapper">
        <div class="banner1">

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

.top-left-wrapper {
  display: flex;
  width: 100%;
}

.banner1 {
  height: 140px;
  width: 331px;
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/booking_com_ccd40dc0.jpg");
}

.banner2 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  height: 140px;
  width: 338px;
  background-color: #fff;
}

.banner2-title {
  display: block;
    padding: 0 30px 5px 0;
    margin: 0;
    font-size: 16px;
    font-weight: 700;
    color: #c6007e;
    text-transform: uppercase;
}

.banner2-content {
  margin-top: 0;
  margin-bottom: 2rem;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-size: 1rem;
  line-height: 1.5;
  font-weight: 400;
}

strong {
  color: #c6007e;
}
</style>
