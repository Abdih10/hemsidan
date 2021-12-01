<template>
  <Navigation />
  <div class="home">
    <h1>This is the home page!</h1>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "../components/Navigation.vue";

@Options({
  components: {
    Navigation,
  },
})
export default class Home extends Vue {}
</script>
