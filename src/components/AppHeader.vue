<template>
  <div class="header">
    <b-container>
      <!-- class="align-items-center" -->
      <b-row>
        <b-col cols="3">
          <b-img
            class="border-right pr-20 mr-20"
            :src="require('../assets/images/hamburger.png')"
          ></b-img>
          <b-navbar-brand to="#" class="p-0 m-0">
            <b-img :src="require('../assets/images/logo.png')"> </b-img>
          </b-navbar-brand>
        </b-col>
        <!-- class="d-flex justify-content-center" -->
        <b-col cols="6">
          <b-nav
            class="header__nav justify-content-between font-14 font-weight-bold"
          >
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
        <!-- class="d-flex justify-content-end align-items-center" -->
        <b-col cols="3">
          <b-link to="#">
            <b-icon icon="cart-fill" class="mr-5" aria-hidden="true"></b-icon>
            <div class="d-inline-block text-uppercase font-12 font-weight-bold">
              Cart <span class="header__cart-count">0</span>
            </div>
          </b-link>
          <b-button pill variant="outline-secondary" class="ml-20"
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

.header {
  &__nav {
    .nav-item {
      margin-right: 20px;
      &:last-child {
        margin-right: 0;
      }
    }
    .nav-link {
      padding: 0 5px;
      color: $color-light-text;
    }
    .nav-link:hover,
    .nav-link:focus {
      color: $color-text;
    }
  }
  &__cart-count {
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
