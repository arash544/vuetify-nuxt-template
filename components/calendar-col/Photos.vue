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
  margin-top: 40px;
  margin-left: 148px;
  line-height: 1.3;
  width: 60%;
  @media only screen and (max-width: 768px) {
    margin-top: 20px;
    margin-left: -312px;
    width: 100vw;
    z-index: -1000;
    text-align: center;
  }
}

img {
  width: 10%;
  margin: -5px;
  &:hover {
    transform: scale(2);
  }
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
  p {
    font-family: $bodytext;
  }
}
</style>