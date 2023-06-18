<template>
  <div class="slider-title">
    <span>Event Galleries</span>
  </div>
  <swiper :navigation="true" :modules="modules" class="mySwiper">
    <swiper-slide v-for="(slide, index) in info" :key="slide.id">
      <img :src="slide.download_url" alt="Slide-Image" />
      <span class="swiper-slide__text">SLIDE {{ index + 1 }}</span>
    </swiper-slide>
  </swiper>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";
import axios from "axios";
// Import Swiper styles
import "swiper/css";

import "swiper/css/navigation";

// import required modules
import { Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation],
    };
  },
  data() {
    return {
      info: null,
    };
  },
  mounted() {
    axios
      .get("https://picsum.photos/v2/list?page=2&limit=100")
      .then((response) => {
        this.info = response.data;
        //console.log(this.info)
      })
      .catch((error) => console.log(error));
  },
};
</script>

<style>
.mySwiper {
  background-color: #2f363d;
  border-radius: 15px;
  margin: 0 5vw;
}

.slider-title {
    font-size: 4.28vw;
    padding-bottom: 1vw;
  }
.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #c4c4c4;
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 60vw;
  object-fit: cover;
}
.swiper-button-prev::after {
  content: url("../assets/images/arrow-prev.svg");
  position: relative;
  top: 20.35vw;
}
.swiper-button-next::after {
  content: url("../assets/images/arrow-next.svg");
  position: relative;
  top: 20.35vw;
}
.swiper-slide__text {
  position: absolute;
  font-size: 5.5vw;
  top: calc(45vw + 10px);
}
@media screen and (min-width: 990px) {
  .slider-title {
    text-align: left;
    font-size: 1.8vw;
    padding: 0.3vw 0;
  }
  .swiper-slide img {
    height: 100%;
  }

  .mySwiper {
    margin: 0;
    height: 27vw;
  }

  .swiper-slide__text {
    position: absolute;
    font-size: 1.137vw;
    top: calc(22.5vw);
  }
  .swiper-button-prev::after {
    position: absolute;
    top: 9.5vw;
    left: 12vw;
  }
  .swiper-button-next::after {
    position: absolute;
    top: 9.5vw;
    left: -12vw;
  }
}
</style>
