<template>
  <div id="app">
    <AppHeader></AppHeader>
    <TopBar></TopBar>
    <AppBanner></AppBanner>
    <div class="content-wrapper pt-50 pb-50">
      <TopFilter class="mb-30"></TopFilter>
      <div class="container">
        <div class="row">
          <div class="col-3">
            <SideBar></SideBar>
          </div>
          <div class="col-9">
            <Product></Product>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import TopBar from "./components/TopBar.vue";
import AppBanner from "./components/AppBanner.vue";
import TopFilter from "./components/TopFilter.vue";
import SideBar from "./components/SideBar.vue";
import Product from "./components/Product.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    TopBar,
    AppBanner,
    TopFilter,
    SideBar,
    Product,
  },
};
</script>
<style>
.content-wrapper {
  background-color: #e4e5e7;
}
</style>
