<template>
  <div class="responsive-wrap">
    <div class="wrapper">
      <div class="box box1">
        Wizz Air Hungary Ltd.
      </div>
      <div class="box box2">
        All rights reserved.
      </div>
      <div class="box box3">
        © 2004–2018 Wizz Air
      </div>
      <div class="box box4">
        © 2000–2018 Navitaire
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
  width: 100%;
  background-color: #06038d;
  display: flex;
  justify-content: center;
}

.wrapper {
  width: 100%;
  max-width: 1400px;
  display: flex;
  text-align: left;
  height: 44px;
  padding-top: 15px;
  padding-bottom: 15px;
  font-size: 14px;
  font-weight: 700;
  margin-top: 30px;
  color: #fff;
}

.box {
  display: inline;
}

.box {
  margin-left: 20px;
}

@media only screen and ( max-width:905px) {
  .box {
    margin: 0;
    width: 25%;
  }
}

@media only screen and ( max-width:610px) {
  .wrapper {
    height: 80px;
  }
}

</style>
