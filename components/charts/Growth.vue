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
  width: 30%;
  height: 170px;
  background-color: rgb(239, 248, 186);
  box-shadow: $shadow;
  position: absolute;
  top: 820px;
  left: 61.5%;
  transform: translate(-50%, -50%);
  @media only screen and (max-width: 768px) {
    margin-top: 600px;
    margin-left: -61.32px;
    width: 100%;
    position: absolute;
    
  }
}
.parent h3 {
  padding: 30px;
  position: absolute;
}
.parent img {
  width: 55%;
  margin: auto;
}
.imgparent {
  text-align: center;
  margin: auto;
  display: block;
}
</style>