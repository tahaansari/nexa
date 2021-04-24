<template>
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
</template>

<script>
export default {};
</script>

<style></style>
