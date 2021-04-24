<template>
  <div class="app-header">
    <b-container>
      <b-row class="align-items-center">
        <b-col cols="3" class="d-flex align-items-center">
          <b-img
            class="border-right pt-35 pb-35 pr-35 mr-35"
            :src="require('../assets/images/hamburger.png')"
          ></b-img>
          <b-navbar-brand to="#" class="p-0 m-0">
            <b-img :src="require('../assets/images/logo.png')"> </b-img>
          </b-navbar-brand>
        </b-col>
        <b-col cols="6">
          <b-nav class="header__nav justify-content-between font-14">
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
        <b-col cols="3 d-flex justify-content-end align-items-center">
          <b-link to="#">
            <b-icon icon="cart-fill" class="mr-5" aria-hidden="true"></b-icon>
            <div class="d-inline-block text-uppercase font-12">
              Cart <span class="app-header__cart">0</span>
            </div>
          </b-link>
          <b-button pill variant="outline-secondary" class="ml-20 px-15 py-10"
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
@import "../assets/scss/variables.scss";
.app-header {
  .nav-link {
    padding: 5px 10px;
  }
  &__cart {
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
}
</style>
