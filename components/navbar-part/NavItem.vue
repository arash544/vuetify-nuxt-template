<template>
  <li>
    <v-icon class="icon">{{item.icon}}</v-icon>
    <span>{{item.title}}</span>
  </li>
</template>

<script>
export default {
  name: "NavItem",
  props: {
    item: {
      type: Object,
      required: true
    }
  }
};
</script>

<style lang="scss" scoped>
li {
  // margin-left: 10px;
  padding: 10px;
  border-radius: 8px;
  margin-bottom: 20px;
  
  span,
  .icon {
    color: rgb(68, 62, 62);
    padding: 2px;
    //   :active,
    // :hover,
    // :focus {
    //   background-color: blueviolet;
    //   color: white;
    // }
  }
    // :active,
    // :hover,
    // :focus {
    //   background-color: blueviolet;
    //   color: white;
    // }
}
</style>