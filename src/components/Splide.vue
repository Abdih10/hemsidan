<!-- Det här är en tredje part plugin som jag har laddat ner till projektet för att skapa slides för nyhterna som ska vara i. -->
<!-- https://splidejs.com/integration/vue-splide/ -->
<template>
  <div class="carousel-inner relative w-full overflow-">
    <div class="carousel-item active relative float-left w-full">
      <h2>Nyheter</h2>

      <Splide :options="options" has-slider-wrapper>
        <SplideSlide>
          <img src="" />
        </SplideSlide>

        <SplideSlide>
          <img src="" />
        </SplideSlide>

        <SplideSlide>
          <img src="" />
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
      pauseOnHover: true,
      arrows: "slider",
      height: "15rem",
    };
    return {
      options,
    };
  },
});
</script>
