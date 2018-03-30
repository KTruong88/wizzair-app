<template>
  <div class="responsive-wrap">
    <div class="wrapper">

      <div class="header">
        Airports and Tourism
      </div>

      <div class="content-wrapper">
        <div class="link link1">
          Visit Catania
        </div>
        <div class="link link2">
          Visit Tel Aviv from Debrecen
        </div>
        <div class="link link3">
          Visit Cyprus
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

.responsive-wrap {
  width: 100%;
  display: flex;
  justify-content: center;
}

.wrapper {
  display: flex;
  max-width: 1400px;
  width: 100%;
  flex-direction: column;
  background-color: #fff;
  height: 127px;
  margin: 0 40px;
  padding: 0 20px;
}

.header {
  font-size: 14px;
  font-weight: 700;
  color: #343434;
  text-transform: uppercase;
  text-align: left;
  padding: 0;
  margin: 40px 0 20px;
  font-family: P22 Underground Pro,sans-serif;
}

.content-wrapper {
  display: flex;
  justify-content: flex-start;
  width: 100%;
}

.link {
  width: 272px;
  height: 38px;
  display: block;
  padding-bottom: 4px;
  line-height: 1.4;
  color: #919191;
  text-decoration: none;
  font-size: 14px;
  text-align: left;
}

.link:hover {
  cursor: pointer;
}

@media only screen and ( max-width:700px) {
  .responsive-wrap {
    margin-top: -50px;
    height: 170px;
  }

  .content-wrapper {
    flex-direction: column;
  }
}

@media only screen and ( max-width:500px) {
  .header, .content-wrapper {
    display: none;
  }
}

</style>
