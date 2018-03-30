<template>
  <div class="responsive-wrap">
    <div class="wrapper">
      <div class="box, box1">
        <div class="box1-img">

        </div>

          <div class="content-wrapper">
            <div class="title title1">
              Need help?
            </div>
            <div class="content content1">
              <a href="">Browse our FAQ to get instant answer</a>
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
        <div class="title">
          Never miss a good deal
        </div>
        <div class="content content3">
          Subscribe to our newsletter and be the first to know about new routes and special offers.
        </div>
        <button class="subscribe-btn">
          Subscribe
        </button>
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
}

.wrapper {
  display: flex;
  margin: 0 40px;
  width: 100%;
  max-width: 1400px;
  align-self: center;
}

.box {
  flex: 1;
}

.box1, .box2, .box3 {
  display: flex;
  height: 140px;
  margin-top: -300px;
  flex-wrap: wrap;
  padding: 0 30px;
  border-right: 1px solid #e1e1e1;
}

.content-wrapper {
  text-align: left;
  margin-left: 120px;
  margin-top: -112px;
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
  text-align: left;
}

/* Middle Box */

.box1, .box2, .box3 {
  height: 140px;
  width: 459px;
}

.content2 {
  margin-top: -15px;
  text-align: left;
}

.content2, .content3 {
  line-height: 20px;
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

.subscribe-btn {
  display: inline-block;
  text-decoration: none;
  margin-top: 20px;
  min-width: 150px;
  padding: 15px 20px;
  font-size: 14px;
  background-color: #c6007e;
  font-family: P22 Underground Pro,sans-serif;
  color: #fff;
  text-align: center;
  text-transform: uppercase;
  white-space: normal;
  vertical-align: middle;
  cursor: pointer;
  border-radius: 3px;
}

.box3 {
  border-right: none;
}

.content3 {
  text-align: left;
}

@media only screen and ( max-width:1155px) {
  .wrapper {
    margin-top: 50px;
  }
}

@media only screen and ( max-width:1035px) {
  .box1-img {
    background-size: 80%;
    background-repeat: no-repeat;
  }

  .title {
    text-align: left;
  }
}

@media only screen and ( max-width:831px) {
  .wrapper {
    flex-wrap: wrap;
  }
  .box {
    flex-basis: 100%;
  }
  .box1-img {
    background-size: 100%;
  }
  .box1, .box2 {
    border-right: none;
    border-right: 0;
    border-bottom: 1px solid #e1e1e1;
  }
  .box1 {
    margin-top: -650px;
  }
  .box2 {
    margin-top: -500px;
    padding-botom: 20px;
    height: 180px;
  }
}

</style>
