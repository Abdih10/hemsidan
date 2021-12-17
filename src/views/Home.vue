<template>
  <Navigation />
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
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "../components/Navigation.vue";
import VueCal from "vue-cal";
import "vue-cal/dist/vuecal.css";

@Options({
  components: {
    Navigation,
    VueCal,
  },
})
export default class Home extends Vue {}
</script>
