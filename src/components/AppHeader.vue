<template>
  <div class="header">
    <b-container>
      <b-row class="align-items-center">
        <b-col cols="3">
          <b-img
            class="border-right pt-7 pb-7 pr-7 mr-7"
            :src="require('../assets/images/hamburger.png')"
          ></b-img>
          <b-navbar-brand href="#">
            <b-img :src="require('../assets/images/logo.png')"> </b-img>
          </b-navbar-brand>
        </b-col>
        <b-col cols="6" class="d-flex justify-content-center">
          <b-nav class="font-14 header__nav font-weight-bold">
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
        <b-col cols="3" class="d-flex justify-content-end align-items-center">
          <b-link to="#">
            <b-icon icon="cart-fill" class="mr-1" aria-hidden="true"></b-icon>
            <div class="d-inline-block text-uppercase font-12 font-weight-bold">
              Cart <span class="cart-count">0</span>
            </div>
          </b-link>
          <b-button pill variant="outline-secondary" class="ml-4"
            >Sign In</b-button
          >
        </b-col>
      </b-row>
    </b-container>
    <div class="border-top">
      <b-container>
        <!-- align-items-center -->
        <b-row class="">
          <b-col cols="8">
            <b-nav class="text-uppercase font-12 ml-n2 py-2 font-weight-bold">
              <b-nav-item to="#">Top sales</b-nav-item>
              <b-nav-item to="#">Brand Focus</b-nav-item>
              <b-nav-item to="#">Hi-tech</b-nav-item>
              <b-nav-item to="#">Best sellers</b-nav-item>
              <b-nav-item to="#">Projects</b-nav-item>
            </b-nav>
          </b-col>
          <b-col cols="4">
            <div class="d-flex align-items-center h-100">
              <b-link
                href="#foo"
                class="mr-4 border-right font-weight-bold text-uppercase font-12"
                >Support</b-link
              >
              <div
                class="d-flex align-items-center border-left border-right px-3 h-100"
              >
                <b-icon-search></b-icon-search>
                <b-form-input
                  type="text"
                  placeholder="I’m looking for ..."
                  required
                  class="border-0 font-weight-bold color-light-text"
                >
                </b-form-input>
              </div>
            </div>
          </b-col>
        </b-row>
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
