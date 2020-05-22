<template>
  <div class="button-parent">
    <button class="btn-1">Start Course</button>
    <button class="btn-2">Reschedule</button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.button-parent {
  margin-left: 1350px;
  margin-top: -60px;
  width: 40%;

  @media only screen and (max-width: 768px) {
    margin-top: 20px;
    margin-left: -94px;
    margin-right: -14px;
    width: 100vw;
    z-index: -1000;
    text-align: center;
  }
}
.btn-1 {
  background-color: $primary;
  color: white;
}
.btn-2 {
  border: 1px solid gray;
}
.btn-1,
.btn-2 {
  outline: none;
  margin-right: 15px;
  padding: 10px;
  border-radius: 30px;
}
</style>