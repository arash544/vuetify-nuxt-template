<template>
  <div class="calendar-wrapper">
    <v-date-picker v-model="date" class="mt-4 calendar"></v-date-picker>
    <v-date-picker
      v-model="date"
      full-width
      :landscape="$vuetify.breakpoint.smAndUp"
      class="mt-4 cal"
    ></v-date-picker>
  </div>
</template>

<script>
export default {
  name: "Calendar",
  data() {
    return {
      picker: new Date().toISOString().substr(0, 10)
    };
  }
};
</script>

<style lang="scss" scoped>
.calendar-wrapper {
  width: 21%;
  padding-left: 30px;
  @media only screen and (max-width: 768px) {
    width: 100vw;
    margin-left: -109px;
  }
}
.calendar {
  box-shadow: $shadow;
  width: 100%;

  @media only screen and (max-width: 768px) {
    display: none;
  }
}
.cal {
  @media only screen and (max-width: 768px) {
    margin-top: 20px;
    width: 100vw;
    z-index: -1000;
  }
  @media only screen and (min-width: 768px) {
    display: none;
  }
}
</style>
<style>
/* .v-picker__title{
  color:#000 !important;
} */
</style>