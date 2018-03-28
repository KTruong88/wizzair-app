<template>
  <div class="wrapper">
    <h1 class="title">
      Cheap flight offers**
    </h1>

    <div class="cards-container">
        <div>
          <b-card class="cards card1">
            <div class="card-content-wrapper">
              <div class="card-text-wrapper">
                  <p class="card-title">
                    Budapest
                  </p>
                <p class="card-content">
                  from Baku**
                </p>
              </div>
              <p class="price">‎​
                €​44.99
              </p>
            </div>
          </b-card>
        </div>

        <div>
          <b-card class="cards card2">
            <div class="card-content-wrapper">
              <div class="card-text-wrapper">
                  <p class="card-title">
                    Timisoara
                  </p>
                <p class="card-content">
                  from London Luton**
                </p>
              </div>
              <p class="price">‎​
                €​20.99
              </p>
            </div>
          </b-card>
        </div>

        <div>
          <b-card class="cards card3">
            <div class="card-content-wrapper">
              <div class="card-text-wrapper">
                  <p class="card-title">
                    Warsaw
                  </p>
                <p class="card-content">
                  from Malta**
                </p>
              </div>
              <p class="price">‎​
                €​39.99
              </p>
            </div>
          </b-card>
        </div>
        <div class="disclaimer-wrap">
          <p>**One way price including taxes, administration and other non-optional charges and one hand luggage (max: 55x40x23cm). Each piece of checked-in baggage is subject to additional fees. The price applies only to bookings made on wizzair.com and the WIZZ mobile app or made by our call centre. Number of seats at indicated prices are limited.</p>
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
  width: 100%;
  flex-direction: column;
  max-width: 1450px;
  background-color: #f2f2f2;
  height: 500px;
  margin-top: -10px !important;
}

.cards-container {
  display: flex;
  width: 100%;
  padding: 0 20px;
  margin: 0 auto;
  max-width: 1400px;
  justify-content: space-between;
  flex-wrap: wrap;
}

.title {
  font-size: 24px;
  font-weight: 300;
  padding: 0 40px;
  color: #06038d;
  margin-bottom: 30px;
  width: 100%;
  margin-top: 40px;
  text-align: left;
}

.cards {
  max-width: 442px;
  height: 250px;
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 8px;
}

.cards:hover {
  cursor: pointer;
}

.card1 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/bud_1_6f5475bf.jpg");
}

.card2 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/tsr_5d6c8fbf.jpg");
}
.card3 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/waw_7ef0c47c.jpg");
}
.card4 {
  background-image: URL("https://wizzair.com/static/images/default-source/banner-images/plq_0f0e3515.jpg");
}

.card-text-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.card-title-wrapper {
  padding: 0 10px 0 20px;
  font-weight: 700;
  font-family: P22 Underground Pro,sans-serif;
  font-size: 16px;
  color: #c6007e;
  text-transform: uppercase;
  width: 442px;
}

.card-title {
  margin-top: 10px;
  font-family: P22 Underground Pro,sans-serif;
  font-weight: 700;
  text-shadow: none;
  font-size: 16px;
  color: #c6007e;
  text-transform: uppercase;
  margin-bottom: 0px;
}

.card-content-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0 10px 0 20px;
  vertical-align: middle;
  background-color: #fff;
  width: 442px;
  height: 100px;
  margin-left: -21px;
  margin-top: 129px;
}

.card-content {
  font-size: 14px;
  text-shadow: none;
}

.price {
  align-self: flex-end;
  font-size: 20px;
  font-weight: 700;
  color: #06038d;
}

.disclaimer-wrap {
  margin-top: 35px;
  text-align: left;
}

@media only screen and ( max-width:1395px) {
  .cards, .card-content-wrapper {
    width: 400px;
  }
}

@media only screen and ( max-width:1270px) {
  .cards, .card-content-wrapper {
    width: 350px;
  }
}

@media only screen and ( max-width:1225px) {
  .cards, .card-content-wrapper {
    width: 320px;
  }
}

@media only screen and ( max-width:1025px) {
  .card1, .card2, .card-content-wrapper {
    width: 400px;
  }

  .card3 {
    display: none;
  }
}

@media only screen and ( max-width:870px) {
  .card1, .card2, .card-content-wrapper {
    width: 300px;
  }
}

@media only screen and ( max-width:660px) {
  .card1, .card2, .card-content-wrapper {
    width: 250px;
  }
}

@media only screen and ( max-width:550px) {
  .card1, .card2, .card-content-wrapper {
    display: none;
  }

  .disclaimer-wrap {
    display: none;
  }

  .wrapper {
    display: none;
  }

  .title {
    display: none;
  }
}

</style>
