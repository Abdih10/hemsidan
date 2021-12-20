<template>
  <ContactForm />
  <Rapport />
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Rapport from "@/components/Rapport.vue";
import ContactForm from "../components/ContactForm.vue";
@Options({
  components: {
    ContactForm,
    Rapport,
  },
})
export default class Utryckningsrapporter extends Vue {}
</script>
