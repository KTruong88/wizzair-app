<template>
  <div class="responsive-wrap">
    <div class="wrapper">
      <b-navbar id="navbar" toggleable="md" type="dark" variant="info">

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand id="logo" href="/">
        <img src="https://wizzair.com/static/assets/images/wizz-logo--white_e5edffeb.svg" alt="">
      </b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <!-- Right aligned nav items -->
        <b-navbar-nav type="light" class="ml-auto">

          <b-nav-item class="nav-item padding"     v-on:click="openPlan()">
            Plan
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right>
            Information
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right>
            Check In & Bookings
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right>
            Sign In
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item right>
            <span class="flag padding"></span>English
          </b-nav-item>
        </b-navbar-nav>

      </b-collapse>
      </b-navbar>
    </div>

    <div>
      <div v-if="plan" class="plan-modal-wrapper">
        <div class="plan-modal">

          <div class="title-wrap">
            <div class="modal-title">
              Explore your travel opportunities
            </div>
            <div class="close-icon-div" v-on:click="closePlan()">
              <icon name="close" class="close-icon"></icon>
            </div>
          </div>

          <b-row>
            <b-col class="box box1" cols="4">
              <div class="box-img box-img1">

              </div>
              <div class="content-wrap">
                <div class="content">
                  <p class="box-title">
                    Select flight
                  </p>
                  <p class="box-content">
                    Book flights to your Wizz Air destination of choice on your ideal departure date.
                  </p>
                </div>
              </div>
            </b-col>

            <b-col class="box" cols="4">
              <div class="box-img box-img2">

              </div>
              <div class="content-wrap">
                <div class="content">
                  <p class="box-title">
                    Fare finder
                  </p>
                  <p class="box-content">
                    Flexible with dates? Search for the lowest available fare for your journey, and book by best price.
                  </p>
                </div>
              </div>
            </b-col>

            <b-col class="box" cols="4">
              <div class="box-img box-img3">

              </div>
              <div class="content-wrap">
                <div class="content">
                  <p class="box-title">
                    Timetable
                  </p>
                  <p class="box-content">
                    Find out our flight schedule to your chosen destination and select our lowest fare available for your travel date.
                  </p>
                </div>
              </div>
            </b-col>
          </b-row>

          <b-row>
            <b-col class="box box4" cols="4">
              <div class="box-img box-img4">

              </div>
              <div class="content-wrap">
                <div class="content">
                  <p class="box-title">
                    Destination Map
                  </p>
                  <p class="box-content">
                    Explore our expanding network of flight routes and see how far Wizz Air can take you.
                  </p>
                </div>
              </div>
            </b-col>

              <b-col class="box box5" cols="4">
                <div class="box-img box-img5">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Destinations
                    </p>
                    <p class="box-content">
                      Browse our list of destinations and choose your favourite place for your next holiday.
                    </p>
                  </div>
                </div>
              </b-col>

              <b-col class="box box6" cols="4">
                <div class="box-img box-img6">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Trip Planner
                    </p>
                    <p class="box-content">
                      Discover our destinations and be inspired, from great budget breaks to the best beach holidays.
                    </p>
                  </div>
                </div>
              </b-col>
            </b-row>

        </div>
      </div>
    </div>
  </div>


</template>

<script>

export default {
  name: 'navbar',
  data() {
    return {
      plan: false
    }
  },
  methods: {
    openPlan() {
      this.plan = true
    },
    closePlan() {
      this.plan = false
    }
  }
}
</script>

<style scoped>

.row {
  margin: 0 40px;
}

.plan-modal-wrapper {
  display: flex;
  position: absolute;
  flex-direction: column;
  height: 383vh;
  width: 100%;
  z-index: 9988;
  background-color: rgba(0,0,0,.5);
}

.plan-modal {
  display: flex;
  width: 100%;
  max-width: 1445px;
  align-self: center;
  flex-direction: column;
  height: 100vh;
  background-color: #fff;
}

.wrapper {
  width: 100%;
}

.title-wrap {
  display: flex;
  max-width: 1400px;
  align-self: center;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  border-bottom: 1px solid #e1e1e1;
  height: 100px;
}

.modal-title {
  margin: 0 20px;
  font-size: 40px;
  font-weight: 300;
  color: #06038d;
  text-transform: uppercase;
  padding: 20px 0 0;
  margin-bottom: 10px;
}

.close-icon {
  width: 40px;
  height: 40px;
}

.close-icon-div {
  color: #c6007e;
  margin-right: 20px;
}

.close-icon:hover {
  cursor: pointer;
}

.content-wrap {
  display: flex;
  flex-direction: column;
}

.box {
  display: flex;
  align-items: center;
  /*padding: 0 20px;*/
}

.box-title {
  display: inline-block;
  margin: 0 0 5px;
  color: #c6007e;
  font-size: 14px;
  font-weight: 700;
  text-transform: uppercase;
  padding: 0;
  margin: 40px 0 20px;
  font-family: P22 Underground Pro,sans-serif;
  align-self: flex-start;
  margin-left: 40px;
}

.box-content {
  padding: 0;
  font-size: 16px;
  line-height: 1.5;
  color: #343434;
  text-align: left;
  margin-left: 40px;
  margin-top: -12px;
}

.box-img {
  height: 100px;
  width: 100px;
  background-repeat: no-repeat;
  background-size: 100%;
  margin-top: 40px;
  margin-right: -15px;
}

.box-img1 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/airplane_d05b5739.png");
}
.box-img2 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/fare-finder-icon_15e0126b.png");
}
.box-img3 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/fare-finder-icon_15e0126b.png");
}
.box-img4 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/destination-map-icon_6cfacbb1.png");
}
.box-img5 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/fligts-all-destinations-icon_9ead75e9.png");
}
.box-img6 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/trip_planner_icon_6f589cab.png");
}
.content {
  display: flex;
  flex-direction: column;
}

#navbar {
  margin-top: -60px;
  height: 65px;
}

#logo {
  margin-left: 2%;
}

.item-divider {
  width: 2px;
  height: 30px;
  background-color: #201dbc;
}

.nav-item {
  font-size: 12px;
  font-family: Source Sans Pro, sans-serif;
  height: 45px;
  line-height: 25px;
}

.padding {
  padding-right: 10px;
  padding-left: 10px;
  font-weight: 520;
}

.nav-item:hover {
  text-decoration-line: underline;
}

.bg-info {
  background-color: #06038d !important;
}

.navbar-dark .navbar-nav .nav-link {
  color: #fff;
  text-transform: uppercase;
  font-size: 12px;
  white-space: nowrap;
}

.flag {
  width: 5px;
  height: 5px;
  background-image: url('http://www.w3.org/2000/svg');
}

</style>
