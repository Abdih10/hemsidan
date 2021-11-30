<template>
  <div class="home">
    <h1>This is the home page!</h1>
  </div>
  <Splide />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Splide from "@/components/Splide.vue"; // @ is an alias to /src

@Options({
  components: {
    Splide,
  },
})
export default class Home extends Vue {}
</script>
