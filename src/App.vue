<template>
  <div class="flex flex-col h-screen">
    <header>
      <Navigation />
    </header>
    <div clas="fixed inset-x-0 bottom-0 p-4">
      <Footer />
    </div>
    <router-view />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navigation from "./components/Navigation.vue";
import Footer from "./components/Footer.vue";

@Options({
  components: {
    Navigation,
    Footer,
  },
})
export default class App extends Vue {}
</script>
