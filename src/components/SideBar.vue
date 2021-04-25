<template>
  <div class="side-bar">
    <div class="accordion mb-30" role="tablist">
      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-1>Top Sales</div>
        </b-card-header>
        <b-collapse
          id="accordion-1"
          visible
          accordion="my-accordion"
          role="tabpanel"
        >
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>

      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-2>Brand Focus</div>
        </b-card-header>
        <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>

      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-3>Hi-Tech</div>
        </b-card-header>
        <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>
    </div>

    <div class="accordion" role="tablist">
      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-1>Available</div>
        </b-card-header>
        <b-collapse
          id="accordion-1"
          visible
          accordion="my-accordion"
          role="tabpanel"
        >
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>

      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-2>Brands</div>
        </b-card-header>
        <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>

      <b-card no-body>
        <b-card-header class="side-bar__item" role="tab">
          <div block v-b-toggle.accordion-3>Hi-Tech</div>
        </b-card-header>
        <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
          <b-card-body class="p-0">
            <b-link class="side-bar__subitem" to="#foo">Cell Phones </b-link>
            <b-link class="side-bar__subitem" to="#foo">Cameras </b-link>
            <b-link class="side-bar__subitem" to="#foo">Computers </b-link>
            <b-link class="side-bar__subitem" to="#foo">Tv, Audio </b-link>
            <b-link class="side-bar__subitem" to="#foo">Video Games</b-link>
          </b-card-body>
        </b-collapse>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: `
          Anim pariatur
        `,
    };
  },
};
</script>

<style lang="scss">
.side-bar {
  &__item {
    padding: 10px 20px;
    text-transform: uppercase;
    font-size: 14px;
  }
  &__subitem {
    font-size: 12px;
    display: block;
    padding: 10px 20px;
    background: #f0f2f7;
    color: #a1a8bd;
    border-bottom: 1px solid #dfe4ee;
    font-weight: 400;
    text-transform: uppercase;
    &:last-child {
      border-bottom: none;
    }
  }
}
</style>
