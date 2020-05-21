<template>
  <nav>
    <ul>
      <NavItem v-for="(itm,index) in list" :key="index" :item="itm" />
    </ul>
    <div class="nav img">
      <img src="avatar.png" alt />
    </div>
    <div class="nav-txt">
      <h3>Lorem, ipsum.</h3>
      <p>Lorem ipsum dolor sit amet consectetur.</p>
    </div>
    <v-btn class="btn-icon" icon>
      <v-icon class="icon" large>mdi-arrow-right-bold-circle-outline</v-icon>
    </v-btn>
  </nav>
</template>

<script>
import NavItem from "./NavItem";
export default {
  name: "Nav",
  components: {
    NavItem
  },
  data() {
    return {
      list: [
        {
          title: "Dashboard",
          icon: "mdi-view-dashboard-variant"
        },
        {
          title: "My Courses",
          icon: "mdi-fire"
        },
        {
          title: "Ebooks",
          icon: "mdi-text"
        },
        {
          title: "Lessons",
          icon: "mdi-clock"
        },
        {
          title: "Messages",
          icon: "mdi-message"
        },
        {
          title: "Rewards",
          icon: "mdi-credit-card"
        },
        {
          title: "Settings",
          icon: "mdi-cog"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>

nav {
  position: fixed;
  width: 11%;
  left: 0px;
  top: 0;
  bottom: 0;
  font-family:$nav ;
  @media only screen and (max-width: 768px) {
    display: none;
  }
  .nav-txt {
    margin-top: 20px;
  }
  img {
    width: 80%;
  }

  h3,
  p {
    text-align: center;
    line-height: 1.2;
    font-family: $bodytext;
  }
  h3 {
    color: $red;
  }
  p {
    color: $lightgray;
  }

  ul {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    padding-top: 100px;
    
    cursor: pointer;

    :active,
    :hover,
    :focus {
      background-color: $primary;
      color: white;
    }
  }
  .btn-icon{
      margin-top: 50px;
      margin-left: 80px;
  }
}
</style>