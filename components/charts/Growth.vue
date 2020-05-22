<template>
  <div class="parent">
    <h3>Growth</h3>
    <div class="imgparent">
      <img src="growth.png" alt />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.parent {
  width:123%;
  height: 190px;
  background-color: rgb(239, 248, 186);
  box-shadow: $shadow;
  margin-top: 22px;
  @media only screen and (max-width: 768px) {
    margin-top: 20px;
    margin-left: -114px;
    width: 100vw;
    z-index: -1000;
  }
}
.parent h3 {
  padding: 30px;
  position: absolute;
}
.parent img {
  width: 55%;
  margin: auto;
  @media only screen and (max-width: 768px) {
    width: 45%;
  }
}
.imgparent {
  text-align: center;
  margin: 20px auto;
  display: block;
  @media only screen and (max-width: 768px) {
    margin: 10px auto;
  }
}
</style>