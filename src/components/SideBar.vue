<template>
  <div class="accordion" role="tablist">
    <b-card no-body>
      <b-card-header role="tab">
        <div block v-b-toggle.accordion-1>Accordion 1</div>
      </b-card-header>
      <b-collapse
        id="accordion-1"
        visible
        accordion="my-accordion"
        role="tabpanel"
      >
        <b-card-body>
          <b-card-text
            >I start opened because <code>visible</code> is
            <code>true</code></b-card-text
          >
          <b-card-text>{{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body>
      <b-card-header role="tab">
        <div block v-b-toggle.accordion-2>Accordion 2</div>
      </b-card-header>
      <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text
            >I start opened because <code>visible</code> is
            <code>true</code></b-card-text
          >
          <b-card-text>{{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body>
      <b-card-header role="tab">
        <div block v-b-toggle.accordion-3>Accordion 3</div>
      </b-card-header>
      <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text
            >I start opened because <code>visible</code> is
            <code>true</code></b-card-text
          >
          <b-card-text>{{ text }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
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

<style></style>
