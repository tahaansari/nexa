<template>
  <div class="filter">
    <b-container>
      <div class="filter__wrapper">
        <div class="d-flex justify-content-between">
          <div>
            <label for="">Sort By:</label>
            <b-form-select v-model="selected" :options="sortby"></b-form-select>
          </div>
          <div>
            <label for="">
              Keywords
            </label>
            <b-form-input
              class="rounded-pill filter__keywords"
              v-model="text"
              placeholder="Tablet"
            ></b-form-input>
            <label for="">
              Price
            </label>
            <b-form-input
              class="rounded-pill filter__price"
              v-model="text"
              placeholder="From"
            ></b-form-input>
            -
            <b-form-input
              class="rounded-pill filter__price"
              v-model="text"
              placeholder="To"
            ></b-form-input>
            <b-form-checkbox
              class="filter__freeshipping"
              v-model="status"
              value="accepted"
              unchecked-value="not_accepted"
            >
              Free Shipping
            </b-form-checkbox>
          </div>
          <div>
            <label for="">
              Ship to:
            </label>
            <b-form-select v-model="selected" :options="shipto"></b-form-select>
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: null,
      sortby: [
        { value: null, text: "Best match" },
        { value: "a", text: "Best match" },
        { value: "b", text: "Best match" },
      ],
      shipto: [
        { value: null, text: "Usa" },
        { value: "a", text: "Usa" },
        { value: "b", text: "Usa" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variable.scss";
</style>
