<template>
  <div class="text-parent">
    <h6>Today</h6>
    <h4>Basic Marketing</h4>
    <p>Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took.</p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.text-parent {
  position: absolute;
  right: 60px;
  top: 520px;
  width: 15%;
  height: 90px;
  line-height: 1.3;

  @media only screen and (max-width: 768px) {
    margin-top: 1000px;
    margin-right: -59.5px;
    width: 100%;
    position: absolute;
    padding: 10px;
    text-align: center;
  }
}
h6 {
  color: $red;
  font-size: 15px;
}
p {
  color: $lightgray;
}
h3,
p,
h6 {
  font-family: $bodytext;
}
</style>