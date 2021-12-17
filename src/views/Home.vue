<template>
  <div class="home">
    <h1>This is the home page!</h1>
  </div>
  <Sections />
  <Footer />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "../components/Navigation.vue";
import Sections from "../components/Sections.vue";
import Footer from "../components/Footer.vue";

@Options({
  components: {
    Navigation,
    Sections,
    Footer,

  },
})
export default class Home extends Vue {}
</script>
