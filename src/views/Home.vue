<template>
  <div class="home">
    <h1>This is the home page!</h1>
  </div>
  <vue-cal
    :time="false"
    hide-weekends
    class="vuecal--rounded-theme vuecal--blue-theme"
    style="width: 600px; height: 400px"
  ></vue-cal>
  />
  <Sections />
  <Footer />

</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "../components/Navigation.vue";
import VueCal from "vue-cal";
import "vue-cal/dist/vuecal.css";
import Sections from "../components/Sections.vue";
import Footer from "../components/Footer.vue";


@Options({
  components: {
    Navigation,
    VueCal,
    Sections,
    Footer,
  },
})
export default class Home extends Vue {}
</script>
