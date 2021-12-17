<template>
  <main>
    <Splide />
    <VueCalendar />
    <Sections />
  </main>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Splide from "../components/Splide.vue";
import VueCalendar from "../components/VueCalendar.vue";
import Sections from "../components/Sections.vue";

@Options({
  components: {
    Splide,
    VueCalendar,
    Sections,
  },
})
export default class Home extends Vue {}
</script>
