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

          <b-nav-item class="nav-item padding"          v-on:click="openPlan()">
            Plan
            <span class="arrow"></span>
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right
            v-on:click="openInfo()">
            Information
            <span class="arrow"></span>
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
            <span class="flag padding"></span>
            English
            <span class="arrow"></span>
          </b-nav-item>
        </b-navbar-nav>

      </b-collapse>
      </b-navbar>
    </div>

<!-- *******************Plan Modal******************** -->


      <div v-if="modal == 0" class="plan-modal-wrapper">
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




            <div class="title-wrap">
              <div class="modal-title">
                Organize your whole holiday easily
              </div>
            </div>

            <b-row>
              <b-col class="box box7" cols="4">
                <div class="box-img box-img7">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Flight + Hotel
                    </p>
                    <p class="box-content">
                      Book flights and hotels together with Wizz Tours and save time and money on your perfect getaway.
                    </p>
                  </div>
                </div>
              </b-col>

              <b-col class="box box8" cols="4">
                <div class="box-img box-img8">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Hotels
                    </p>
                    <p class="box-content">
                      Reserve your hotel with Booking.com and get 10% of your booking value back as WIZZ credit.
                    </p>
                  </div>
                </div>
              </b-col>

              <b-col class="box box9" cols="4">
                <div class="box-img box-img9">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Cars
                    </p>
                    <p class="box-content">
                      Rent a car with Rentalcars.com
                    </p>
                  </div>
                </div>
              </b-col>
            </b-row>

            <b-row>
              <b-col class="box box10" cols="4">
                <div class="box-img box-img10">

                </div>
                <div class="content-wrap">
                  <div class="content">
                    <p class="box-title">
                      Airport Transfer
                    </p>
                    <p class="box-content">
                      More than 100 routes, prices starting from €2/person.
                    </p>
                  </div>
                </div>
              </b-col>

                <b-col class="box box11" cols="4">
                  <div class="box-img box-img11">

                  </div>
                  <div class="content-wrap">
                    <div class="content">
                      <p class="box-title">
                        Airport parking
                      </p>
                      <p class="box-content">
                        Save up to 60% - reserve it now!
                      </p>
                    </div>
                  </div>
                </b-col>
              </b-row>

          </div>
        </div>

<!-- *******************Information Modal******************** -->

    <div v-if="modal == 1" >
      <div class="info-modal">


        <div class="info-title-wrap">
          <div class="info-modal-title">
            asdfsd
          </div>
          <div class="info-close" v-on:click="closeInfo()">
            <icon name="close" class="info-close-icon"></icon>
          </div>
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
      modal: null,
    }
  },
  methods: {
    openPlan() {
      this.modal = 0
    },
    closePlan() {
      this.modal = null
    },
    openInfo() {
      this.modal = 1
    },
    closeInfo() {
      this.modal = null
    }
  }
}
</script>

<style scoped>




/***********Plan Modal***********/

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
}

.box:hover {
  cursor: pointer;
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
  background-size: object-fit;
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
.box-img7 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/flight-and-hotel_bc20d94b.png");
}
.box-img8 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/hotels-icon_cdf2f217.png");
}
.box-img9 {
  margin-right: -55px;
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/car-icon_d4ab4364.png");
}
.box-img10 {
  margin-right: -55px;
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/small-icons/parking-icon_d4c080bc.png");
}
.box-img11 {
  margin-right: -55px;
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/small-icons/airport-transfer-icon_3358badc.png");
}

.content {
  display: flex;
  flex-direction: column;
}





/***********Info Modal***********/

.info-modal-wrapper {
  display: flex;
  position: absolute;
  flex-direction: column;
  height: 383vh;
  width: 100%;
  z-index: 9988;
  background-color: rgba(0,0,0,.5);
}

.info-modal {
  display: flex;
  width: 100%;
  max-width: 1445px;
  align-self: center;
  flex-direction: column;
  height: 100vh;
  background-color: #fff;
}

/*.info-title-wrap {

}

.info-modal-title {

}

.info-close {

}

.info-close-icon {

}*/











/***********Navbar***********/




#navbar {
  margin-top: -60px;
  height: 65px;
}

#logo {
  margin-left: 2%;
}

.arrow {
  display: inline-block;
  margin-left: 2px;
  vertical-align: middle;
  border: 4px solid transparent;
  border-top-color: currentColor;
  content: "";
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
