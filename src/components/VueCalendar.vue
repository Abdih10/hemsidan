<template>
  <div>
    <vue-cal
      class="vuecal--blue-theme"
      selected-date="2021-12-17"
      :time-from="9 * 60"
      :time-to="20 * 60"
      :disable-views="['years', 'year']"
      active-view="week"
      hide-weekends
      events-on-month-view="short"
      :events="events"
      style="height: 600px"
    >
      >
    </vue-cal>
  </div>
</template>
<script>
import VueCal from "vue-cal";
import "vue-cal/dist/vuecal.css";

export default {
  components: { VueCal },
  data: () => ({
    minEventWidth: 0,
    events: [
      {
        start: "2021-12-13 08:00",
        end: "2021-12-13 10:00",
        title: "Morgonmöte",
        content: '<i class="v-icon material-icons">sentiment_satisfied_alt</i>',
        class: "Möte",
      },
      {
        start: "2021-12-15 10:30",
        end: "2021-12-15 12:00",
        title: "Another thing",
        content: '<i class="v-icon material-icons">thumb_up</i>',
        class: "blue-event",
      },
      {
        start: "2021-12-17 13:00",
        end: "2021-12-27 14:30",
        title: "Redovisning",
        content: '<i class="v-icon material-icons">fikarumet</i>',
        class: "Möte",
      },
    ],
  }),
};
</script>
