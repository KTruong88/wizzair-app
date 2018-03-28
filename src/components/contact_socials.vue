<template>
  <div class="wrapper">
    <div class="box, box1">
      <div class="box1-img">

      </div>
      <div class="content-wrapper">
        <div class="title">
          Need help?
        </div>
        <div class="content">
          <a href="">Browse our FAW to get instant answer</a>
        </div>
      </div>
    </div>

    <div class="box, box2">
      <div class="title">
        On the move?
      </div>
      <div class="content content2">
        Booking a cheap Wizz Air flight ticket has never been so
        easy as with our FREE mobile application.
      </div>
      <div class="box2-img-wrapper">
        <div class="box2-img box2-img1">

        </div>
        <div class="box2-img box2-img2">

        </div>
      </div>
    </div>

    <div class="box, box3">

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
  margin: 0 40px;
}

.box {
  flex: 1;
}

.box1, .box2 {
  display: flex;
  height: 140px;
  margin-top: -300px;
  flex-wrap: wrap;
  padding: 0 30px;
  border-right: 1px solid #e1e1e1;
}

.content-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.box1-img {
  height: 90px;
  width: 99px;
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/qa_a85e5f8e.png");
  background-size: cover;
  margin-right: 30px;
}

.title {
  font-size: 24px;
  font-weight: 300;
  color: #06038d;
  margin-bottom: 10px;
}

.content > a {
  color: #a6006a;
  text-decoration: underline;
  cursor: pointer;
}

/* Middle Box */

.box2 {
  height: 140px;
  width: 459px;
}

.content2 {
  margin-top: -15px;
  text-align: left;
}

.box2-img-wrapper {
  display: flex;
}

.box2-img {
  height: 34px;
  width: 120px;
  background-size: cover;
}

.box2-img:hover {
  cursor: pointer;
}

.box2-img1 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/badge-apple-app-store_64be092d.png");
  margin-right: 10px;
}

.box2-img2 {
  background-image: URL("https://wizzair.com/static/images/default-source/information-services-images/card-images/badge-google-play_9647fa2e.png");
}


</style>
