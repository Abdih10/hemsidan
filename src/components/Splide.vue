<template>
  <div class="wrapper">
    <h2>Autoplay</h2>

    <Splide :options="options" has-slider-wrapper>
      <SplideSlide>
        <img
          src="https://cdn.mos.cms.futurecdn.net/2NBcYamXxLpvA77ciPfKZW-970-80.jpg.webp"
        />
      </SplideSlide>

      <SplideSlide>
        <img
          src="https://heroichollywood.com/wp-content/uploads/2021/02/Zack_Snyder_Justice_League_Henry_Cavill_Superman.jpg"
        />
      </SplideSlide>

      <SplideSlide>
        <img
          src="https://allfilmskases.com/wp-content/uploads/2019/02/iron-man-cool-guys-dont-look-at-explosions-222059.jpg"
        />
      </SplideSlide>

      <template #after-slider>
        <div class="splide__progress">
          <div class="splide__progress__bar"></div>
        </div>

        <div class="splide__autoplay">
          <button class="splide__play">Play</button>
          <button class="splide__pause">Pause</button>
        </div>
      </template>
    </Splide>
  </div>
</template>

<script lang="ts">
import { Options } from "@splidejs/splide";
import { Splide, SplideSlide } from "@splidejs/vue-splide";
import { defineComponent } from "vue";

import "@splidejs/splide/dist/css/themes/splide-skyblue.min.css";

export default defineComponent({
  name: "AutoplayExample",
  components: {
    Splide,
    SplideSlide,
  },
  setup() {
    const options: Options = {
      rewind: true,
      gap: "1rem",
      autoplay: true,
      pauseOnHover: false,
      arrows: "slider",
      height: "15rem",
    };
    return {
      options,
    };
  },
});
</script>
