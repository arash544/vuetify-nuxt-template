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
  margin-top: 20px;
  margin-left: 148px;
  line-height: 1.3;
   width: 60%;

  @media only screen and (max-width: 768px) {
    margin-top: 435px;
    margin-left: -312px;
    width: 100vw;
    z-index:-1000;
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
    @media only screen and (max-width: 768px) {
padding-left:150px ;
padding-right:150px ;
    
  }
}
</style>