<template>
  <div class="icon-parent">
    <div class="icon1">
      <v-icon class="coloricon">mdi-clock</v-icon>
      <p>55 mins</p>
    </div>
    <div class="icon2">
      <v-icon class="coloricon">mdi-message</v-icon>
      <p>03 Lessons</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss"scoped>
.icon-parent {
  margin-top: 20px;
  margin-left: 148px;
  line-height: 1.3;
  width: 60%;
  padding: 15px 5px;
  @media only screen and (max-width: 768px) {
    margin-top: 20px;
    margin-left: -312px;
    width: 100vw;
    z-index: -1000;
    text-align: center;
  }
}
.icon1,
.icon2 {
  margin-bottom: 10px;

  @media only screen and (max-width: 768px) {
    display: inline-block;
    padding: 10px 20px 10px 40px;
  }
}
.coloricon {
  color: $primary;
   &:hover {
    transform: scale(2);
  }
  @media only screen and(max-width: 768px) {
    font-size: 28px;
  }
}
.icon1 p,
.icon2 p {
  margin-left: 10px;;
  display: inline-block;
  font-family: $bodytext;
  @media only screen and(max-width: 768px) {
    font-size: 22px;
  }
}
</style>