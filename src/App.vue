<template>
  <div id="app">
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

<style>
* {
  margin: 0;
  padding: 0;
}
</style>
