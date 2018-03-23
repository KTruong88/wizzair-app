<template>
  <b-navbar id="navbar" toggleable="md" type="dark" variant="info">

  <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

  <b-navbar-brand id="logo" href="/">
    <img src="https://wizzair.com/static/assets/images/wizz-logo--white_e5edffeb.svg" alt="">
  </b-navbar-brand>

  <b-collapse is-nav id="nav_collapse">

    <!-- Right aligned nav items -->
    <b-navbar-nav type="light" class="ml-auto">

      <b-nav-item class="nav-item padding">
        Plan
      </b-nav-item>

      <b-nav-item class="item-divider">
      </b-nav-item>

      <b-nav-item class="nav-item padding" right>
        Information
      </b-nav-item>

      <b-nav-item class="item-divider">
      </b-nav-item>

      <b-nav-item class="nav-item padding" right>
        Check In & Bookings
      </b-nav-item>

      <b-nav-item class="item-divider">
      </b-nav-item>

      <b-nav-item class="nav-item padding" right>
        Sign In
      </b-nav-item>

      <b-nav-item class="item-divider">
      </b-nav-item>

      <b-nav-item right>
        <span class="flag padding"></span>English
      </b-nav-item>
    </b-navbar-nav>

  </b-collapse>
</b-navbar>

</template>

<script>
export default {
  name: 'navbar',
  data() {
    return {
      title: 'Welcome to Wizzair',
    }
  },
  // methods: {
  //
  // }
}
</script>

<style scoped>

#navbar {
  margin-top: -60px;
  height: 60px;
}

#logo {
  margin-left: 2%;
}

.item-divider {
  width: 2px;
  height: 30px;
  background-color: #201dbc;
}

.nav-item {
  font-size: 12px;
  font-family: Source Sans Pro, sans-serif;
  height: 45px;
  line-height: 25px;
}

.padding {
  padding-right: 10px;
  padding-left: 10px;
  font-weight: 520;
}

.nav-item:hover {
  text-decoration-line: underline;
}

.bg-info {
  background-color: #06038d !important;
}

.navbar-dark .navbar-nav .nav-link {
  color: #fff;
  text-transform: uppercase;
  font-size: 12px;
  white-space: nowrap;
}

.flag {
  width: 5px;
  height: 5px;
  background-image: url('http://www.w3.org/2000/svg');
}

</style>
