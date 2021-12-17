<template>
  <Navigation />
  <div class="home">
    <h1>This is the home page!</h1>
  </div>
  <Sections />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "../components/Navigation.vue";
import Sections from "../components/Sections.vue";

@Options({
  components: {
    Navigation,
    Sections,
  },
})
export default class Home extends Vue {}
</script>
