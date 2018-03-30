<template>
  <div class="responsive-wrap">
    <div class="wrapper">
      <div class="col col1">
        <div class="title">
          Services
        </div>

        <div class="link-wrap">
          <a href="">WIZZ Discount Club</a>
          <a href="">WIZZ Flex</a>
          <a href="">WIZZ Priority</a>
          <a href="">Seat allocation</a>
          <a href="">Hotels</a>
          <a href="">Car rentals</a>
          <a href="">Airport transfer</a>
          <a href="">All services and fees</a>
        </div>
      </div>

      <div class="col col2">
        <div class="title">
          Customer Service
        </div>
        <div class="link-wrap">
          <a href="">Booking with Wizz Air</a>
          <a href="">Baggage</a>
          <a href="">Payments</a>
          <a href="">Special Assistance</a>
          <a href="">Online check-in</a>
          <a href="">General Conditions of Carriage</a>
        </div>
      </div>

      <div class="col col3">
        <div class="title">
          Flights & Destinations
        </div>
        <div class="link-wrap">
          <a href="">Current Flight Status</a>
          <a href="">Map</a>
          <a href="">Destinations</a>
          <a href="">Timetable</a>
          <a href="">Cancellation information</a>
        </div>
        <div class="social-media-icons">
          <div class="social-title">
            Follow us
          </div>

          <div class="icon-wrapper">
            <div class="icon icon1">

            </div>
            <div class="icon icon2">

            </div>
            <div class="icon icon3">

            </div>
            <div class="icon icon4">

            </div>
            <div class="icon icon5">

            </div>
          </div>
        </div>
      </div>

      <div class="col col4">
        <div class="title">
          About Wizz Air
        </div>
        <div class="link-wrap">
          <a href="">Company information</a>
          <a href="">News</a>
          <a href="">WIZZ Magazine</a>
          <a href="">Career</a>
          <a href="">Press Office</a>
          <a href="">For travel agents & partners</a>
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

.responsive-wrap {
  display: flex;
  justify-content: center;
  width: 100%;
  background-color: #f2f2f2;
}

.wrapper {
  width: 100%;
  max-width: 1400px;
  height: 259px;
  display: flex;
}

.col {
  display: flex;
  flex-direction: column;
  margin: 0 20px;
}

.title, .social-title {
  margin: 0 0 10px;
  padding: 0;
  font-size: 14px;
  font-weight: 700;
  color: #343434;
  text-transform: uppercase;
  font-family: P22 Underground Pro,sans-serif;
  text-align: left;
}

.title {
  margin-top: 25px;
}

.social-title {
  margin-top: 25px;
}

.link-wrap {
  display: flex;
  flex-direction: column;
  text-align: left;
}

.link-wrap > a {
  overflow: visible;
  line-height: 1.4;
  color: #c6007e;
  text-decoration: none;
  white-space: normal;
  font-size: 14px;
}

.social-media-icons {
  display: flex;
  flex-direction: column;
}
.icon-wrapper {
  display: flex;
}

@media only screen and ( max-width:740px) {
  .wrapper {
    height: 350px;
  }
}

@media only screen and (max-width:700px) {
  .wrapper {
    margin-top: 40px;
    flex-wrap: wrap;
    height: 300px;
    margin-bottom: 180px;
  }
  .link-wrap {
    flex-basis: 100%;
  }
  .icon-wrapper {
    margin-bottom: 30px;
  }
}

@media only screen and (max-width:605px) {
  .wrapper {
    height: 500px;
  }
}

@media only screen and (max-width:500px) {
  .wrapper {
    display: none;
  }
}

</style>
