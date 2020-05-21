<template>
  <div class="button-parent">
      <button class="btn-1">Start Course</button>
      <button class="btn-2">Reschedule</button>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.button-parent{
    position:absolute;
    right: 60px;
    top: 830px;
    /* box-shadow: 0 10px 20px -6px #777; */
    width:15%;
    height: 90px;
    padding:30px 40px;
    
          @media only screen and (max-width: 768px) {
    margin-top: 960px;
    margin-right: -60px;
    width: 100%;
    position: absolute;
    text-align: center;
    height: 70px;
    padding:15px 35px 10px 50px
   
  }
  
   
}
.btn-1{
    background-color:$primary;
    color:white;
    margin-right: 15px;
    padding:10px;
    border-radius: 30px;
 
}
</style>