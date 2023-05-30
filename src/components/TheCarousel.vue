<template>
  <swiper
      :slidesPerView="3"
      :spaceBetween="40"
      :navigation="true"
      :loop="true"
      :pagination="{
      clickable: true,
    }"
      :modules="modules"
  >
    <swiper-slide>
      <div class="slide">
        <div class="background-image"></div>
        <h2>title</h2>
        <p class="mb-5">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco lab
        </p>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slide">
      <div class="background-image"></div>
      <h2>title</h2>
      <p class="mb-5">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco lab
      </p>
    </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slide">
        <div class="background-image"></div>
        <h2>title</h2>
        <p class="mb-5">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco lab
        </p>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slide">
        <div class="background-image"></div>
        <h2>title</h2>
        <p class="mb-5">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco lab
        </p>
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/free-mode';
import 'swiper/css/pagination';
import 'swiper/css/navigation';



// import required modules
import { Navigation,FreeMode, Pagination } from 'swiper';

export default {
  name: 'TheCarousel',
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation, FreeMode, Pagination],
    };
  },
};
</script>

<style lang="scss" scoped>
.slide {
  border-top: 1px solid black;
  border-bottom: 1px solid black;
  width: 385px;
}

.background-image {
  margin-top: 10px;
  height: 325px;
  width: 385px;
  background-color: turquoise;
}
</style>