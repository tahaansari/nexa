<template>
  <div id="app">
    <AppHeader></AppHeader>
    <AppBanner></AppBanner>
    <TopFilter></TopFilter>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBanner from "./components/AppBanner.vue";
import TopFilter from "./components/TopFilter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppBanner,
    TopFilter,
  },
};
</script>
<style></style>
