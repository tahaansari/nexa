<template>
  <div class="border-bottom">
    <b-container>
      <b-row class="align-items-center">
        <b-col cols="3">
          <b-img
            class="border-right p-5 mr-4"
            :src="require('../assets/images/hamburger.png')"
          ></b-img>
          <b-navbar-brand href="#">
            <img src="../assets/images/logo.png" alt="" />
          </b-navbar-brand>
        </b-col>
        <b-col cols="6">
          <b-nav>
            <b-nav-item active>Home</b-nav-item>
            <b-nav-item>Devices</b-nav-item>
            <b-nav-item>Delivery & Payment</b-nav-item>
            <b-nav-item>Garantee</b-nav-item>
            <b-nav-item>About Us</b-nav-item>
          </b-nav>
        </b-col>
        <b-col cols="3">
          <b-icon icon="cart-fill" aria-hidden="true"></b-icon>
          <span class="text-uppercase fs-2">Cart 0</span>
          <b-button pill variant="outline-secondary text-uppercase ml-4"
            >Sign In</b-button
          >
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/scss/variable.scss";
</style>
