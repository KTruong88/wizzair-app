<template>
  <div class="wrapper">
    <div class="container">
      <div class="heading">
        Explore your travel opportunities with WIZZ!
      </div>
      <div class="tools-content">


        <div class="content-item first">
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
        </div>

        <div class="item-divider"></div>

        <div class="content-item second">
          <img class="farefinder-img"       src="https://wizzair.com/static/images/default-source/information-services-images/card-images/fare-finder-icon_90c09a7a.png" alt="farefinder"
          >
          <div class="title-wrap">
            <div class="title">
              Fare Finder
            </div>
            <p class="content">
              619 Routes
            </p>
          </div>
        </div>

        <div class="item-divider"></div>

        <div class="content-item third">
          <div class="title">

          </div>
          <p class="content"></p>
        </div>


        <div class="content-item fourth">
          <div class="title">

          </div>
          <p class="content"></p>
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

</style>
