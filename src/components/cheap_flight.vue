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
  max-width: 1400px;
  padding: 0 20px;
  margin: 0 auto;
  background-color: #f2f2f2;
  height: 900px;
}

.cards-container {
  display: flex;
  justify-content: space-between;
}

.title {
  margin-top: 20px;
  font-size: 24px;
  font-weight: 300;
  color: #06038d;
  align-self: flex-start;
  margin-bottom: 30px;
}

.cards {
  max-width: 442px;
  width: 442;
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

</style>
