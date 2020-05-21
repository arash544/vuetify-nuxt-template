<template>
  <div class="photo-parent">
    <img src="facebook.png" alt />
    <img src="pintrest.png" alt />
    <img src="instagram.png" alt />
    <img src="soundcloud.png" alt />
    <img src="Twitter.png" alt />
    <p>Lorem ipsum dolor.</p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.photo-parent {
  position: absolute;
  right: 60px;
  top: 650px;
  width: 15%;
  height: 50px;
  line-height: 1.2;
  @media only screen and (max-width: 768px) {
    margin-top: 975px;
    margin-right: -60px;
    width: 100%;
    position: absolute;
    text-align: center;
    height: 70px;
  }
}

img {
  width: 10%;
  margin: -5px;
  @media only screen and (max-width: 768px) {
    padding-top: 10px;
    width: 7%;
  }
}
.photo-parent p {
  display: inline-block;
  margin-left: 4px;
  color: $lightgray;
  @media only screen and (max-width: 768px) {
    display: block;
    padding-top: 5px;
    font-size: large;
  }
  p{
    font-family: $bodytext;
  }
}
</style>