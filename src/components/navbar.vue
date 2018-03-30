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

          <b-nav-item class="nav-item padding"          @click="openPlan()">
            Plan
            <span class="arrow"></span>
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right
            @click="openInfo()">
            Information
            <span class="arrow"></span>
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right @click="openBooking()">
            Check In & Bookings
          </b-nav-item>

          <b-nav-item class="item-divider">
          </b-nav-item>

          <b-nav-item class="nav-item padding" right @click="openSignIn()">
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

<div v-if="modal == 1" class="plan-modal-wrapper  info-modal-wrapper">
  <div class="plan-modal info-modal">

    <div class="title-wrap info-title-wrap">
      <div class="modal-title info-modal-title">
        Information & Services
      </div>

      </input>
      <div class="close-icon-div" v-on:click="closePlan()">
        <icon name="close" class="close-icon"></icon>
      </div>
    </div>

    <b-row class="info-row info-row-top">
      <b-col class="info-box info-box1" cols="3">
        <div class="info-box-title">
          Booking Information
        </div>

        <div class="info-box-content">
          <ul class="info-box-list">
            <li>How to book</li>
            <li>Children and infants</li>
            <li>Payments</li>
            <li>Check-in and boarding</li>
            <li>Changing your reservation</li>
            <li>Group bookings</li>
            <li>Mobile</li>
          </ul>
        </div>
      </b-col>

      <b-col class="info-box info-box2" cols="3">
        <div class="info-box-title">
          Prices & Discounts
        </div>

        <div class="info-box-content">
          <ul class="info-box-list">
            <li>Fare Finder</li>
            <li>Fares & Bundles</li>
            <li>All service & fees</li>
            <li>Refunds and Compensations</li>
            <li>Billing guide</li>
            <li>Baggage fee calculator</li>
          </ul>
        </div>
      </b-col>

      <b-col class="info-box info-box3" cols="3">
        <div class="info-box-title">
          Wizz Services
        </div>

        <div class="info-box-content">
          <ul class="info-box-list">
            <li>Convenience options</li>
            <li>WIZZ Discount Club</li>
            <li>Fare Lock</li>
            <li>Privilege Pass</li>
            <li>WIZZ Priority</li>
            <li>WIZZ Flex</li>
            <li>On-time Guarantee</li>
            <li>WIZZ for families</li>
            <li>WIZZ Account</li>
            <li>Gift Voucher</li>
            <li>Flexile travel partner</li>
          </ul>
        </div>
      </b-col>

      <b-col class="info-box info-box4" cols="3">
        <div class="info-box-title">
          About Us
        </div>

        <div class="info-box-content">
          <ul class="info-box-list">
            <li>Company Information</li>
            <li>News</li>
            <li>Investor relations</li>
            <li>Press Office</li>
            <li>WIZZ Magazine</li>
            <li>General Conditions of Carriage</li>
            <li>Privacy policy</li>
          </ul>
        </div>
      </b-col>
    </b-row>

    <b-row class="info-row">
      <b-col class="info-box info-box5" cols="3">
        <div class="info-box-title">
          Travel Information
        </div>

        <div class="info-box-content">
          <ul class="info-box-list">
            <li>Baggage</li>
            <li>Electronic devices on board</li>
            <li>Seat allocation</li>
            <li>Travel documents</li>
            <li>Onboard services</li>
            <li>Travelling with infants and babies</li>
            <li>Cancellation information</li>
          </ul>
        </div>
      </b-col>

        <b-col class="info-box info-box6" cols="3">
          <div class="info-box-title">
            Flight Status
          </div>

          <div class="info-box-content">
            <ul class="info-box-list">
              <li>Current flight status</li>
            </ul>
            <br>
          <div class="info-box-title">
            FAQ
          </div>
          <ul class="info-box-list">
            <li>Frequently Asked Questions</li>
          </ul>
          </div>
        </b-col>

        <b-col class="info-box info-box7" cols="3">
          <div class="info-box-title">
            Partner Services
          </div>

          <div class="info-box-content">
            <ul class="info-box-list">
              <li>Travel Insurance</li>
              <li>Hotels</li>
              <li>Car rental</li>
              <li>Airport Parking</li>
              <li>Airport Transfer</li>
              <li>WIZZ Credit Card</li>
              <li>Partner services</li>
            </ul>
          </div>
        </b-col>

        <b-col class="info-box info-box7" cols="3">
          <div class="info-box-title">
            Career
          </div>

          <div class="info-box-content">
            <ul class="info-box-list">
              <li>Work with Us</li>
              <li>Pilots</li>
              <li>Cabin crew/Flight attendant</li>
              <li>Office and Maintenance Positions</li>
            </ul>
            <br>

            <div class="info-box-title">
              Contact
            </div>
            <ul class="info-box-list">
              <li>Contact us</li>
            </ul>
          </div>
        </b-col>
      </b-row>
    </div>
  </div>


<!-- *************Booking Modal************** -->


  <div v-if="modal == 2" class="plan-modal-wrapper  booking-modal-wrapper">
    <div class="plan-modal booking-modal">

      <div class="booking-title-wrap">
        <div class="booking-modal-title">
          Find Booking
        </div>

        <div class="close-icon-div" v-on:click="closeBooking()">
          <icon name="close" class="close-icon"></icon>
        </div>
      </div>

        <div class="booking-modal-body">
          <input class="booking-input input1"
                 type="text"
                 placeholder="Confirmation code"
           >
         </input>

          <input class="booking-input input2"
                 type="text"
                 placeholder="Passenger's last name"
            >
          </input>

          <button class="btn booking-btn" type="button">
            Search
          </button>
        </div>

        <div class="booking-modal-footer">
          <p class="footer-title">
            Already have an account?
          </p>
          <button class="btn booking-btn-login" type="button">
            Log in
          </button>
        </div>

    </div>
  </div>



  <!-- *************Sign in************** -->


    <div v-if="modal == 3" class="plan-modal-wrapper  booking-modal-wrapper">
      <div class="plan-modal booking-modal">

        <div class="booking-title-wrap">
          <div class="booking-modal-title">
            Sign in
          </div>

          <div class="close-icon-div" @click="closeSignIn()">
            <icon name="close" class="close-icon"></icon>
          </div>
        </div>

          <div class="booking-modal-body sign-body">
            <input class="booking-input input1 sign-in-input"
                   type="text"
                   placeholder="E-mail"
             >
           </input>

            <input class="booking-input input2 sign-in-input"
                   type="text"
                   placeholder="Password"
              >
            </input>
            <div class="forgot sign-footer-links">
              <p class="forgot-link">Forgot your password?</p>
            </div>

            <button class="btn booking-btn sign-in-btn sign-in-btn1" type="button">
              Sign in
            </button>
            <button class="btn booking-btn sign-in-btn sign-in-btn2" type="button">
              Cancel
            </button>
          </div>

          <div class="sign-footer">

            <div class="sign-footer-links">
              <div class="link1">
                Registration
              </div>
              <div class="link2">
                Agency Login
              </div>
            </div>
          </div>

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
    },
    openBooking() {
      this.modal = 2
    },
    closeBooking() {
      this.modal = null
    },
    openSignIn() {
      this.modal = 3
    },
    closeSignIn() {
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
  height: 120vh;
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

.info-title-wrap {
  border-bottom: none !important;
  margin-bottom: 25px;
}

.info-box {
  display: flex;
  flex-direction: column;
}

.info-box-title {
  text-transform: uppercase;
  margin: 0 0 10px;
  font-size: 14px;
  font-weight: 700;
  color: #343434;
  text-align: left;
}

.info-box-list {
  overflow: visible;
  line-height: 1.75;
  color: #c6007e;
  text-decoration: none;
  white-space: normal;
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 14px;
  vertical-align: baseline;
  list-style: none;
  text-align: left;
}

.info-row {
  margin: 0 25px;
}

.info-row-top {
  margin-bottom: 40px;
}




/***********Booking Modal************/





.booking-modal {
  position: fixed;
  top: 50%;
  left: 50%;
  z-index: 90;
  width: 480px;
  max-height: calc(100vh - 35vh);
  min-height: calc(100vh - 35vh);
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  background: #fff;
  border-radius: 5px;
  opacity: 1;
  -webkit-transform: translate(-50%,-50%);
  -ms-transform: translate(-50%,-50%);
  transform: translate(-50%,-50%);
  box-shadow: 0 15px 25px rgba(0,0,0,.1);
  -webkit-transition: opacity .5s ease,-webkit-transform .5s ease;
  transition: opacity .5s ease,-webkit-transform .5s ease;
  transition: transform .5s ease,opacity .5s ease;
  transition: transform .5s ease,opacity .5s ease,-webkit-transform .5s ease;
}

.booking-title-wrap {
  display: flex;
  max-width: 1400px;
  align-self: center;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  border-bottom: 1px solid #e1e1e1;
  height: 85px;
  min-height: 85px;
  padding: 30px 20px 30px 65px;
  background: #f2f2f2;
  border-radius: 5px 5px 0 0;
  margin-bottom: 32px;
}

.booking-modal-title {
  font-size: 24px;
  font-weight: 300;
  margin-left: 10px;
  color: #06038d;
}

.booking-modal-body {
  display: flex;
  flex-direction: column;
  border-bottom: 1px solid #e1e1e1;
  height: 238px;
  min-height: 238px;
}

.booking-btn {
  min-width: 150px;
  padding: 10px 20px;
  font-size: 14px;
  background-color: #c6007e;
  position: relative;
  display: inline-block;
  height: 44px;
  min-height: 44px;
  min-width: 180px;
  font-weight: 400;
  width: 70%;
  align-self: center;
  font-family: P22 Underground Pro,sans-serif;
  color: #fff;
  text-align: center;
  text-transform: uppercase;
  white-space: normal;
  vertical-align: middle;
  cursor: pointer;
  border-radius: 3px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.booking-input {
  position: relative;
  z-index: 1;
  border-radius: 3px;
  padding: 20px 10px;
  overflow: hidden;
  white-space: nowrap;
  width: 70%;
  align-self: center;
  padding: 28px 10px 12px;
  font-family: Source Sans Pro,sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 20px;
  color: #343434;
  background-color: #fff;
  border: 1px solid #919191;
  -webkit-transition: padding .2s ease-in-out;
  transition: padding .2s ease-in-out;
  border-radius: 3px;
  margin-bottom: 20px;
  line-height: 20px;
}

.booking-modal-footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 141px;
  min-height: 141px;
}

.footer-title {
  font-size: 12px;
  font-weight: 700;
  color: #343434;
  text-transform: uppercase;
  font-family: Source Sans Pro,sans-serif;
}

.booking-btn-login {
  background-color: #c6007e;
  min-width: 150px;
  font-weight: 400;
  width: 150px;
  min-height: 44px;
  height: 44px;
  align-self: center;
  padding: 10px 20px;
  font-size: 14px;
  font-family: P22 Underground Pro,sans-serif;
  color: #fff;
  text-align: center;
  text-transform: uppercase;
  white-space: normal;
  vertical-align: middle;
  cursor: pointer;
  border-radius: 3px;
}

.btn:hover {
  opacity: .6;
  color: rgba(255, 255, 255, 1);
  box-shadow: 0 5px 15px rgba(145, 92, 182, .4);
}





/***********Sign in***********/






 .sign-in-input {
  height: 62px;
}

.sign-in-btn1 {
  margin-bottom: 10px;
}

 .sign-in-btn2 {
  background-color: #3434e0;
  margin-top: 10px;
}

.sign-body {
  height: 468px;
  border-bottom: none;
}

.sign-footer {
  height: 80px;
}

.forgot {
  margin-top: -18px;
  margin-left: 85px;
}

.sign-footer-links {
  width: 100%;
  display: flex;
  justify-content: space-around;
  padding: 0 45px;
  font-size: 12px;
  font-weight: 700;
  color: #a6006a;
  text-decoration: underline;
  text-transform: uppercase;
}

.sign-footer-links:hover {
  cursor: pointer;
}





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

@media only screen and (max-width:1000px) {

/***** Page Modal******/

  .title-wrap {
    margin-top: 30px;
    padding-bottom: 30px;
  }
  .modal-title {
    text-align: left;
  }
  .plan-modal {
    height: 1300px;
  }
  .row {
    flex-wrap: wrap;
  }
  .col-4 {
    max-width: 50%;
  }
  .box {
    flex-basis: 50%;
  }

/*Info Modal*/

  .col-3 {
    max-width: 50%;
  }
  .info-box {
    flex-basis: 50%;
  }
  .info-box {
    margin-bottom: 20px;
  }
}

@media only screen and (max-width:700px) {

/* Page Modal*/

  .plan-modal-wrapper {
    height: 5200px;
  }
  .title-wrap {
    margin-top: 35px;
    padding-bottom: 35px;
  }
  .modal-title {
    text-align: left;
  }
  .plan-modal {
    height: 1850px;
  }
  .col-4 {
    max-width: 100%;
  }
  .box {
    flex-basis: 100%;
  }

/***** Info Modal******/

  .info-modal {
    height: 2050px;
  }
  .col-3 {
    max-width: 100%;
  }
  .info-box {
    flex-basis: 100%;
  }
  .info-box {
    margin-bottom: 20px;
  }
}

@media only screen and (max-width:540px) {
  .plan-modal {
    height: 2200px;
  }
  .title-wrap {
    margin-top: 90px;
    padding-bottom: 90px;
  }
}

@media only screen and (max-width:500px) {
  .booking-modal {
    width: 370px;
  }
  .forgot-link {
    margin-right: 80px;
  }
}

</style>
