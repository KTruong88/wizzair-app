<template>
  <div class="wrapper">

    <div class="box-wrap box-wrap1">
      <div class="box box1">

      </div>
      <div class="content">
        <p class="title">
          Even prices go better together!
        </p>
        <p class="text">
          Book flights. Book a hotel. Book together & save money at Wizz Tours!
        </p>
      </div>
    </div>

    <div class="box-wrap box-wrap2">
      <div class="box box2">

      </div>
      <div class="content content2">
        <p class="title">
          Airport Transfer
        </p>
        <p class="text">
          More than 100 routes, prices starting from €2/person.
        </p>
      </div>
    </div>

    <div class="box-wrap box-wrap3">
      <div class="box box3">

      </div>
      <div class="content">
        <p class="title">
                          Gift Voucher
        </p>
        <p class="text">
          Surprise your loved ones with a gift they will never forget!

        </p>
      </div>
    </div>

    <div class="box-wrap box-wrap4">
      <div class="box box4">

      </div>
      <div class="content">
        <p class="title">
          Airport Parking
        </p>
        <p class="text">
          Save up to 60% - reserve it now!
        </p>
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
  justify-content: space-between;
  width: 100%;
  flex-wrap: wrap;
  height: 510px;
  background-color: #f2f2f2;
  padding: 0 40px;
  margin: 0 auto;

}

.box-wrap {
  display: flex;
  flex-direction: column;
}

.box {
  height: 227px;
  width: 325px;
  background-size: 100%;
  border-radius: 3px;
}

.content {
  border-bottom-left-radius: 3px;
  border-bottom-right-radius: 3px;
}

.box:hover {
  cursor: pointer;
}

.box1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/br18wizwt09-01-legjobb-ajanlatok-banner-180320_c8e81eea.jpg");
}

.box2 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/picture_2b1cb10d.jpg");
}

.box3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/voucher_home_redesign_5a497654.jpg");
}

.box4 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/3rd-party-banners/airport-parking_18d6c32c.jpg");
}

.content {
  display: flex;
  flex-direction: column;
  height: 107px;
  width: 325px;
  background-color: #fff;
  margin-top: -107px;
  line-height: 16px;
}

.content:hover {
  cursor: pointer;
}

.title {
  display: block;
  padding: 0 30px 5px 0;
  margin: 0;
  font-size: 16px;
  font-weight: 700;
  color: #c6007e;
  text-transform: uppercase;
  text-align: left;
  margin-top: 15px;
  margin-left: 15px;
}

.text {
  display: block;
  min-height: 40px;
  font-size: 14px;
  color: #343434;
  text-align: left;
  margin-left: 15px;
}

@media only screen and (max-width:1420px) {
  .box, .content {
    width: 300px;
  }
}

@media only screen and (max-width:1315px) {
  .box, .content {
    width: 260px;
  }
}

@media only screen and (max-width:1155px) {
  .box, .content {
    width: 480px;
  }
}

@media only screen and (max-width:1055px) {
  .box, .content {
    width: 450px;
  }
  .wrapper {
    height: 600px;
  }
}

@media only screen and (max-width:995px) {
  .box, .content {
    width: 420px;
  }
}

@media only screen and (max-width:935px) {
  .box, .content {
    width: 390px;
  }
}

@media only screen and (max-width:875px) {
  .box, .content {
    width: 360px;
  }

  .box1, .box2 {
    margin-top: 50px;
  }
}

@media only screen and (max-width:830px) {

  .wrapper {
    height: 1090px
  }
  .box1, .box2 {
    margin-top: 220px;
  }
  .box3, .box4 {
    margin-top: -290px;
  }
}

@media only screen and (max-width:815px) {

  .box, .content {
    width: 330px;
  }
}

@media only screen and (max-width:755px) {
  .box, .content {
    width: 300px;
  }
}

@media only screen and (max-width:700px) {
  .box, .content {
    width: 600px;
  }

  .box-wrap1 {
    margin-top: 10px;
  }

  .box-wrap2 {
    margin-top: -350px;
    margin-bottom: 100px;
  }

  .box-wrap3 {
    margin-top: 60px;
    margin-bottom: 100px;
  }



  .wrapper {
    height: 1500px;
  }


}

</style>
