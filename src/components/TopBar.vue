<template>
  <div class="top-bar border-top">
    <b-container>
      <b-row class="align-items-center">
        <b-col cols="8">
          <b-nav class="text-uppercase font-12 ml-n10 py-2 ">
            <b-nav-item to="#">Top sales</b-nav-item>
            <b-nav-item to="#">Brand Focus</b-nav-item>
            <b-nav-item to="#">Hi-tech</b-nav-item>
            <b-nav-item to="#">Best sellers</b-nav-item>
            <b-nav-item to="#">Projects</b-nav-item>
          </b-nav>
        </b-col>
        <b-col cols="4">
          <div class="d-flex align-items-center justify-content-between">
            <b-link to="#foo" class="text-uppercase font-12 py-10 px-20"
              >Support
            </b-link>
            <div
              class="d-flex align-items-center border-left border-right py-10 px-20"
            >
              <b-icon-search></b-icon-search>
              <b-form-input
                type="text"
                placeholder="I’m looking for ..."
                required
                class="border-0 color-light-text"
              >
              </b-form-input>
            </div>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.top-bar {
  .nav-link {
    padding: 5px 10px;
  }
}
</style>
