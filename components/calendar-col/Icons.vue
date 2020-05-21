<template>
  <div class="icon-parent">
<div class="icon1">
    <v-icon class="coloricon">mdi-clock</v-icon>
    <p>55 mins</p>
</div>
<div class="icon2">
    <v-icon class="coloricon" >mdi-message</v-icon>
    <p>03 Lessons</p>
</div>
  </div>
</template>

<script>

export default {

}
</script>

<style lang="scss"scoped>
// @import "./assets/variables.scss";
.icon-parent{
    position:absolute;
    right: 60px;
    top: 720px;
    width:15%;
    height: 90px;
    padding:15px 5px;
      @media only screen and (max-width: 768px) {
    margin-top: 990px;
    margin-right: -60px;
    width: 100%;
    position: absolute;
    text-align: center;
    height: 70px;
   
  }
    
}
.icon1,.icon2{
    margin-bottom: 10px;  
    
    @media only screen and (max-width: 768px) {
    display: inline-block;
    padding:10px 20px 10px 40px;
  }
}
.coloricon{
   
    color:$primary;
}
.icon1 p ,
.icon2 p 
{
    display: inline-block;
    font-family: $bodytext;
}


</style>