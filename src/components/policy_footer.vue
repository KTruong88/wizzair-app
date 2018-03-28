<template>
  <div class="responsive-wrap">
    <div class="wrapper">
      <div class="box box1">
        Privacy Policy
      </div>

      <div class="divider">

      </div>

      <div class="box box2">
        Cookie Policy
      </div>

      <div class="divider">

      </div>

      <div class="box box3">
        Website Terms of Use
      </div>

      <div class="divider">

      </div>

      <div class="box box4">
        Agency Registration
      </div>

      <div class="divider">

      </div>

      <div class="box box5">
        Agency Login
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
  background-color: #040267;
  display: flex;
  justify-content: center;
}

.wrapper {
  height: 44px;
  display: flex;
  padding-top: 15px;
  padding-bottom: 15px;
  font-size: 14px;
  width: 100%;
  max-width: 1400px;
}

.box {
  color: #fff;
  text-decoration: none;
}

.box1 {
  margin-left: 20px;
}

.divider {
  width: 1px;
  height: 20px;
  margin: 0 15px;
  font-weight: 700;
  background-color: #00a1e0;
}

@media only screen and (max-width:770px) {
  .wrapper {
    flex-wrap: wrap;
  }
}

@media only screen and (max-width:685px) {
  .wrapper {
    height: 100px;
  }
  .box5 {
    margin-left: 40px;
  }
}

@media only screen and (max-width:594px) {
  .box5 {
    margin-left: -1px;
  }

}
</style>
