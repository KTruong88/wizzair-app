<template>
  <div class="wrapper">
    <div class="container">
      <div class="heading">
        Explore your travel opportunities with WIZZ!
      </div>
      <div class="tools-content">

        <div class="content-item first">
          <a href="" class="content-links">
            <img class="trip-img" src="https://wizzair.com/static/images/default-source/information-services-images/card-images/trip_planner_icon_e71eb2a9.png" alt="trip-planner"
            >

            <div class="title-wrap">
              <div class="title">
                Trip Planner <span class="pill">New</span>
              </div>
              <p class="content">
                Discover your new favourite place
              </p>
            </div>
          </a>
        </div>

        <div class="item-divider"></div>

        <div class="content-item second">
          <a href="" class="content-links" >
            <img class="farefinder-img"       src="https://wizzair.com/static/images/default-source/information-services-images/card-images/fare-finder-icon_90c09a7a.png" alt="farefinder"
            >
            <div class="title-wrap">
              <div class="title title-fare">
                Fare Finder
              </div>
              <p class="content content-fare">
                619 Routes
              </p>
            </div>
          </a>
        </div>

        <div class="item-divider"></div>

        <div class="content-item third">
          <a href="" class="content-links">
            <img class="map-img" src="https://wizzair.com/static/images/default-source/information-services-images/card-images/destination-map-icon_30dc26c6.png" alt="destination-map icon"
            >

            <div class="title-wrap">
              <div class="title">
                Destination Map
              </div>
              <p class="content">
                146 Destinations in 44 Countries
              </p>
            </div>
          </a>
        </div>

        <div class="item-divider"></div>

        <div class="content-item fourth">
          <a href="" class="content-links">
            <img class="destination" src="https://wizzair.com/static/images/default-source/information-services-images/card-images/fligts-all-destinations-icon_3f3ed902.png" alt="destination"
            >

            <div class="title-wrap">
              <div class="title">
                Destinations
              </div>
              <p class="content">
                Discover our expanding network
              </p>
            </div>
          </a>
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
  padding: 10px 20px 30px;
  margin: 0 0 10px;
  background-color: #fff;
  border-bottom: 1px solid #e1e1e1;
  width: 100%;
  height: 197px;
}

.container {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 1400px;
  padding: 0 20px;
  margin: 0 auto;
  height: 141px;
}

.content-links {
  display: flex;
  text-decoration: none;
  color: inherit;
}

.heading {
  text-align: left;
  font-size: 24px;
  font-weight: 300;
  color: #06038d;
  margin-bottom: 10px;
}

.tools-content {
  display: flex;
  justify-content: center;
}

.trip-img {
  min-width: 100px;
  margin-right: 10px;
}

.farefinder-img {
  min-width: 100px;
  height: 65px;
  margin-top: 10px;
  margin-right: 10px;
}

.map-img {
  min-width: 100px;
  height: 85px;
  margin-top: 10px;
  margin-right: 10px;
  margin-left: 10px;
}

.destination {
  min-width: 100px;
  height: 85px;
  margin-top: 10px;
  margin-right: 10px;
  margin-left: 15px;
}

.content-item {
  display: flex;
  justify-content: center;
  flex: 1;
  height: 97px;
  /*border: 1px solid red;*/
}

.title-wrap {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.title {
  margin-bottom: 5px;
  font-family: P22 Underground Pro,sans-serif;
  color: #c6007e;
  text-transform: uppercase;
  align-self: flex-start;
  font-weight: bold;
}


.pill {
  display: inline-block;
  padding: 3px 5px;
  margin: 0 2px;
  font-size: 10px;
  font-weight: 700;
  color: #fff;
  text-shadow: 0 1px 2px rgba(0,0,0,.1);
  text-transform: uppercase;
  vertical-align: top;
  background-color: #00a1e0;
}

.content {
  margin: 0;
  font-size: 14px;
  line-height: 1;
}

.item-divider {
  width: 1px;
  height: 30px;
  background-color: #e1e1e1;
  align-self: center;
}

@media only screen and (max-width:1180px) {
  .wrapper {
    height: 341px;
  }
  .heading {
    margin-top: 10px;
    margin-left: 65px;
  }
  .tools-content {
    flex-wrap: wrap;
  }
  .content-item {
    flex-basis: 50%;
  }
  .map-img {
    margin-left: -10px;
    margin-top: 30px;
  }
  .destination {
    margin-left: 90px;
    margin-top: 30px;
  }
  .item-divider {
    display: none;
  }

  @media only screen and (max-width:872px) {
    .wrapper {
      height: 577px;
    }
    .heading {
      align-self: center;
      margin-bottom: 20px;
    }
    .content-item {
      flex-basis: 100%;
      justify-content: center;
      margin-top: 10px;
      min-width: 440px;
    }
    .trip-img {

    }
    .farefinder-img {
      margin-top: 30px;
    }
    .trip-img {
      margin-left: 78px;
    }
    .content-fare {
      text-align: left;
    }

    .title {
      margin-top: 30px;
    }
    .farefinder-img {
      margin-left: -28px;
    }
    .map-img {
      margin-left: 70px;
    }
    .destination {
      margin-left: 70px;
    }
  }

  @media only screen and (max-width:410px) {
    .wrapper {
      /*height: 620px;*/
      display: none;
    }
  }

}
</style>
