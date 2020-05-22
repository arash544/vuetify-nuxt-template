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
  padding: 10px;
  border-radius: 8px;
  margin-bottom: 20px;
  list-style-type:none;
  @media only screen and (max-width: 768px) {
    text-align: center;
    transition: all 2s ease-in-out;
  }

  &:hover,
  &:active,
  &:focus {
    span,
    .icon {
      color: #fff;
    }
  }
  span,
  .icon {
    color: rgb(68, 62, 62);
    padding: 2px;
    @media only screen and (max-width: 768px) {
      color: #fff;
    }
  }
}
</style>