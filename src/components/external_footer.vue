<template>
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
</template>

<script>
export default {
}
</script>

<style scoped>

.wrapper {
  display: flex;
  flex-direction: column;
  background-color: #fff;
  height: 127px;
  margin: 0 40px;
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
}

.link:hover {
  cursor: pointer;
}


</style>
