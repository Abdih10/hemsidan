<template>
  <ContactForm />
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
import ContactForm from "../components/ContactForm.vue";
@Options({
  components: {
    ContactForm,
  },
})
export default class Utryckningsrapporter extends Vue {}
</script>
