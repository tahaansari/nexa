<template>
  <div class="filter">
    <b-container>
      <div class="filter__bg">
        <div class="d-flex justify-content-between">
          <div
            class="d-flex align-items-center justify-content-between py-15 px-20 border-right"
          >
            <label class="mb-0 mx-5" for="">Sort By:</label>
            <b-form-select
              class="filter__select filter__select--sort mx-5 ml-40"
              v-model="selected"
              :options="sortby"
            ></b-form-select>
          </div>
          <div class="d-flex justify-content-between py-15 px-20 flex-grow-1">
            <div class="d-flex align-items-center">
              <label class="mb-0 mx-5" for="">
                Keywords
              </label>
              <b-form-input
                class="rounded-pill filter__input filter__input--keywords mx-5"
                v-model="text"
                placeholder="Tablet"
              ></b-form-input>
            </div>

            <div class="d-flex align-items-center">
              <label class="mb-0 mx-5" for="">
                Price
              </label>
              <b-form-input
                class="rounded-pill mx-5 filter__input filter__input--price"
                v-model="text"
                placeholder=""
              ></b-form-input>
              -
              <b-form-input
                class="rounded-pill mx-5 filter__input filter__input--price"
                v-model="text"
                placeholder=""
              ></b-form-input>
            </div>

            <div class="d-flex align-items-center">
              <b-form-checkbox
                class="filter__shipping mx-5"
                v-model="status"
                value="accepted"
                unchecked-value="not_accepted"
              >
                Free Shipping
              </b-form-checkbox>
            </div>
          </div>
          <div
            class="d-flex align-items-center justify-content-between py-15 px-20 border-left"
          >
            <label class="mb-0 mx-5" for="">
              Ship to:
            </label>
            <b-form-select
              class="filter__select filter__select--ship mx-5 ml-40"
              v-model="selected"
              :options="shipto"
            ></b-form-select>
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
@import "../assets/scss/variables.scss";
.filter {
  // &__wrapper {
  //   background-color: #ffffff;
  //   border-radius: 10px;
  // }
  // &__keywords {
  //   width: 160px;
  // }
  // &__price {
  //   width: 60px;
  // }
  // &__freeshipping {
  //   display: inline-block;
  //   min-height: auto;
  //   .custom-control-label::before,
  //   .custom-control-label::after {
  //     top: 50%;
  //     transform: translateY(-50%);
  //   }
  // }
  // label {
  //   margin-bottom: 0;
  //   margin: 0 10px;
  // }
  // input[type="text"] {
  //   display: inline-block;
  //   font-weight: bold;
  //   background: #f0f2f7;
  //   font-size: 12px;
  //   margin: 0 10px;
  //   &::placeholder {
  //     opacity: 0.5;
  //   }
  // }
  // select {
  //   display: inline-block;
  //   width: auto;
  //   font-weight: bold;
  //   text-transform: uppercase;
  //   border: none;
  //   font-size: 12px;
  // }
}
</style>
