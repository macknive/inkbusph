<template>
  <div class="swipes">
    <h2 style="text-align: center">Work Samples</h2>
    <swiper
      :style="{
        '--swiper-navigation-color': '#fff',
        '--swiper-pagination-color': '#fff',
      }"
      :spaceBetween="10"
      :navigation="true"
      :thumbs="{ swiper: thumbsSwiper }"
      :modules="modules"
      class="mySwiper2"
    >
      <swiper-slide><img src="../assets/tat4.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat5.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat6.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat7.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat8.jpg" /></swiper-slide>
    </swiper>
    <swiper
      @swiper="setThumbsSwiper"
      :spaceBetween="10"
      :slidesPerView="4"
      :freeMode="true"
      :watchSlidesProgress="true"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide><img src="../assets/tat11.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat12.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat13.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat14.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat5.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat6.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat7.jpg" /></swiper-slide
      ><swiper-slide><img src="../assets/tat8.jpg" /></swiper-slide>
    </swiper>
  </div>
</template>
<script>
import { ref } from "vue"
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue"

// Import Swiper styles
import "swiper/css"

import "swiper/css/free-mode"
import "swiper/css/navigation"
import "swiper/css/thumbs"

// import required modules
import { FreeMode, Navigation, Thumbs } from "swiper/modules"

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const thumbsSwiper = ref(null)

    const setThumbsSwiper = (swiper) => {
      thumbsSwiper.value = swiper
    }

    return {
      thumbsSwiper,
      setThumbsSwiper,
      modules: [FreeMode, Navigation, Thumbs],
    }
  },
}
</script>

<style scoped>
img {
  max-height: 1200px;
}
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.swiper {
  width: 100%;
  height: 300px;
  margin-left: auto;
  margin-right: auto;
}

.swiper-slide {
  background-size: cover;
  background-position: center;
}

.mySwiper2 {
  height: 80%;
  width: 100%;
}

.mySwiper {
  height: 20%;
  box-sizing: border-box;
  padding: 10px 0;
}

.mySwiper .swiper-slide {
  width: 25%;
  height: 100%;
  opacity: 0.4;
}

.mySwiper .swiper-slide-thumb-active {
  opacity: 1;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

@media screen and (min-width: 450px) {
  .swiper {
    width: 80%;
    height: 100%;
  }
}
</style>
