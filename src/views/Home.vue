<template>
  <div class="home">
    <VueCalendar />
  </div>
  <Sections />
  <Footer />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import VueCalendar from "../components/VueCalendar.vue";
import Sections from "../components/Sections.vue";
import Footer from "../components/Footer.vue";

@Options({
  components: {
    VueCalendar,
    Sections,
    Footer,
  },
})
export default class Home extends Vue {}
</script>
