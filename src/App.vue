<template>
  <div id="app">
    <AppHeader></AppHeader>
    <AppBanner></AppBanner>
    <div class="content-wrapper">
      <TopFilter></TopFilter>
      <div class="container">
        <div class="row">
          <div class="col-3">
            <SideBar></SideBar>
          </div>
          <div class="col-9">
            right content
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBanner from "./components/AppBanner.vue";
import TopFilter from "./components/TopFilter.vue";
import SideBar from "./components/SideBar.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppBanner,
    TopFilter,
    SideBar,
  },
};
</script>
<style>
.content-wrapper {
  background-color: #e4e5e7;
}
</style>
