<template>
  <div class="app-banner">
    <b-carousel
      v-model="slide"
      :interval="4000"
      controls
      indicators
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-20">iPhone 6 32Gb Black</h1>
          <p class="mb-40">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-30 py-12">Buy Now</b-button>
        </b-jumbotron>
      </b-carousel-slide>
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-20">iPhone 6 32Gb Black</h1>
          <p class="mb-40">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-30 py-12">Buy Now</b-button>
        </b-jumbotron>
      </b-carousel-slide>
      <b-carousel-slide :img-src="require('../assets/images/home-banner.jpg')">
        <b-jumbotron bg-variant="transparent text-left p-0 mb-0">
          <h1 class="font-extra-bold mb-20">iPhone 6 32Gb Black</h1>
          <p class="mb-40">
            At first, for some time, I was not able to answer him one word; but
            as he had taken me in his arms I held fast by him, or I should have
            fallen to the ground.
          </p>
          <b-button pill variant="primary px-30 py-12">Buy Now</b-button>
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
.app-banner {
  background-color: #1c1e23;
  .carousel {
    width: 1170px !important;
    margin-left: auto;
    margin-right: auto;
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
    left: 100px;
    top: 50%;
    bottom: auto;
    transform: translateY(-50%);
  }
  .carousel-control-prev {
    display: none;
  }
  .carousel-control-next {
    width: 38px;
    height: 38px;
    padding: 0;
    top: 50%;
    transform: translateY(-50%);
    right: 0;
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
