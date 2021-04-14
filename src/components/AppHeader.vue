<template>
  <div>
    <b-container>
      <b-row class="align-items-center">
        <b-col cols="3">
          <b-img
            class="border-right pt-8 pb-8 pr-8 mr-8"
            :src="require('../assets/images/hamburger.png')"
          ></b-img>
          <b-navbar-brand href="#">
            <b-img :src="require('../assets/images/logo.png')"> </b-img>
          </b-navbar-brand>
        </b-col>
        <b-col cols="6">
          <b-nav class="font-14">
            <b-nav-item>
              Home
            </b-nav-item>
            <b-nav-item>
              Devices
            </b-nav-item>
            <b-nav-item>
              Delivery & Payment
            </b-nav-item>
            <b-nav-item>
              Garantee
            </b-nav-item>
            <b-nav-item>
              About Us
            </b-nav-item>
          </b-nav>
        </b-col>
        <b-col cols="3">
          <b-link to="#">
            <b-icon icon="cart-fill" class="mr-1" aria-hidden="true"></b-icon>
            <div
              class="d-inline-block py-2 text-uppercase font-12 font-weight-bold"
            >
              Cart <span class="cart-count">0</span>
            </div>
          </b-link>
          <b-button
            pill
            variant="outline-secondary text-uppercase ml-4 py-2 px-5 font-12 font-weight-bold"
            >Sign In</b-button
          >
        </b-col>
      </b-row>
    </b-container>
    <div class="border-top">
      <b-container>
        <b-nav class="text-uppercase font-12 ml-n2 pt-1 pb-1">
          <b-nav-item to="#">Top sales</b-nav-item>
          <b-nav-item to="#">Brand Focus</b-nav-item>
          <b-nav-item to="#">Hi-tech</b-nav-item>
          <b-nav-item to="#">Best sellers</b-nav-item>
          <b-nav-item to="#">Projects</b-nav-item>
        </b-nav>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/scss/variable.scss";
.cart-count {
  display: inline-block;
  background: #e3e8f0;
  width: 25px;
  height: 25px;
  border-radius: 50%;
  text-align: center;
  font-weight: bold;
  line-height: 25px;
  margin-left: 5px;
}
</style>
