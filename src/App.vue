<template>
  <div id="app">
    vue cli
    <AppHeader></AppHeader>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>

<style lang="scss">
@import url(./assets/scss/custom.scss);
</style>
