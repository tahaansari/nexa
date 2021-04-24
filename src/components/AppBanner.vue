<template>
  <div>
    <b-carousel
      class="banner-carousel"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#1c1e23"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-3">iPhone 6 32Gb Black</h1>
          <p class="mb-10">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-10 banner-carousel__cta"
            >Buy Now</b-button
          >
        </b-jumbotron>
      </b-carousel-slide>
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-3">iPhone 6 32Gb Black</h1>
          <p class="mb-10">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-10 banner-carousel__cta"
            >Buy Now</b-button
          >
        </b-jumbotron>
      </b-carousel-slide>
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-3">iPhone 6 32Gb Black</h1>
          <p class="mb-10">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-10 banner-carousel__cta"
            >Buy Now</b-button
          >
        </b-jumbotron>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null,
    };
  },
  methods: {
    // slide
    onSlideStart() {
      this.sliding = true;
    },
    // slide
    onSlideEnd() {
      this.sliding = false;
    },
  },
};
</script>

<style lang="scss">
.banner-carousel {
  &__cta {
    padding-top: 13px !important;
    padding-bottom: 13px !important;
  }
  .carousel-inner {
    width: 1400px !important;
    margin-left: auto;
    margin-right: auto;
    padding-left: 15px;
    padding-right: 15px;
  }
  .carousel-control-next-icon {
    padding: 18px;
    border: 1px solid #ffffff;
    border-radius: 50%;
    background-image: url(../assets/images/next-icon.png);
    background-size: 5px;
  }
  .carousel-control-prev-icon {
    display: none;
  }
  .carousel-caption {
    width: 460px;
    left: 5%;
    top: 50%;
    transform: translateY(-50%);
    bottom: auto;
  }
  .carousel-control-next {
    width: 38px;
    height: 38px;
    padding: 0;
    top: 50%;
    transform: translateY(-50%);
    right: 10%;
  }
  .carousel-indicators {
    margin-bottom: 25px;
  }
  .carousel-indicators li {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: transparent;
    border: 1px solid #ffffff;
    margin: 0 4px;
    &.active {
      background: #ffffff;
    }
  }
}
</style>
