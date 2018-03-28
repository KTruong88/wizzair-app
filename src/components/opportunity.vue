<template>
  <div class="wrapper">
    <h1 class="title-wrap">
      <p class="title">Welcome to the world of opportunity</p>
    </h1>

    <div class="card-wrapper">
      <div class="card card1">
        <div class="icon-wrapper icon-wrapper1">

        </div>
        <div class="card-title">
          News
        </div>
        <p class="content">
          Check out the latest company news
        </p>
      </div>

      <div class="card card2">
        <div class="icon-wrapper icon-wrapper2">

        </div>
        <div class="card-title">
          Your Career
        </div>
        <p class="content">
          Check out our open positions and apply now!
        </p>
      </div>

      <div class="card card3">
        <div class="icon-wrapper icon-wrapper3">

        </div>
        <div class="card-title">
          The Freedom of Choice
        </div>
        <p class="content">
          From travelling light to all-in flexibility.
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
  flex-direction: column;
  width: 100%;
  height: 400px;
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
  margin-top: -230px;
  color: #06038d;
  text-align: left;
}

.card-wrapper {
  display: flex;
  justify-content: space-between;
  padding: 0 20px;
  margin-top: -150px;
}

.card {
  display: flex;
  flex-direction: column;
  color: #000;
  text-decoration: none;
  background-color: #fff;
  border-radius: 3px;
  box-shadow: 1px 1px 3px rgba(0,0,0,.25);
  height: 185px;
  width: 442px;
}

.icon-wrapper {
  margin-top: -20px;
  width: 90px;
  height: 90px;
  padding: 10px;
  background-color: #fff;
  border: 1px solid #919191;
  border-radius: 50%;
  box-shadow: 0 8px 10px rgba(0,0,0,.25);
  align-self: center;
  background-size: 55%;
  background-position: center;
  background-repeat: no-repeat;
  align-items: center;
}

.icon-wrapper1 {
  background-image: URL("https://wizzair.com/static/images/default-source/default-library/news-icon_cbe61aba.png");
}

.icon-wrapper2 {
  background-image: URL("https://wizzair.com/static/images/default-source/default-library/career-icon_2690c1ec.png");
}

.icon-wrapper3 {
  background-image: URL("https://wizzair.com/static/images/default-source/default-library/freedom-icon_5ba116de.png");
}

.card-title {
  padding-top: 10px;
  font-weight: 700;
  font-family: P22 Underground Pro,sans-serif;
  font-size: 15px;
  color: #c6007e;
  text-transform: uppercase;
  margin-top: 10px;
  margin-bottom: 7px;
}

.content {
  font-size: 14px;
}

@media only screen and (max-width:1155px) {
  .wrapper {
    height: 600px;
  }
  .title {
    margin-top: 30px;
  }
  .card {
    margin-top: 170px;
  }
}

@media only screen and (max-width:830px) {
  .title {
    margin-top: -340px;
  }
  .card {
    margin-top: -100px;
  }
}

@media only screen and (max-width:700px) {
  .title {
    margin-top: 0;
    z-index: 100;
  }
  .card {
    margin-top: 160px;
  }
}

@media only screen and (max-width:500px) {
  .title, .card, .wrapper {
    display: none;
  }

}
</style>
