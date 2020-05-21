<template>
  <v-row align="center">
    <v-date-picker v-model="date" width="290" class="mt-4 calendar"></v-date-picker>
    <v-date-picker
      v-model="date"
      full-width
      :landscape="$vuetify.breakpoint.smAndUp"
      class="mt-4 cal"
    ></v-date-picker>
  </v-row>
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
.calendar {
  position: absolute;
  right: 70px;
  top: 120px;
  box-shadow: $shadow;

  @media only screen and (max-width: 768px) {
    display: none;
  }
}
.cal {
  @media only screen and (max-width: 768px) {
    margin-top: 80px;

    
  }
  @media only screen and (min-width: 768px) {
    display: none;
  }
}
</style>