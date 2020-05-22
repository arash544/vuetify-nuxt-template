
<template>
  <div class="navbar">
    <v-app-bar color="accent-4" dark class="navbar">
      <template>
        <v-row class="logo">
          <v-btn icon>
            <v-icon large>mdi-domain</v-icon>
            <p class="btnlogo">OnlineOwl</p>
          </v-btn>
        </v-row>
      </template>

      <v-col class="search" cols="5" sm="6" md="3">
        <v-text-field label="Search"></v-text-field>
      </v-col>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-bell</v-icon>
      </v-btn>

      <v-menu left bottom>
        <template v-slot:activator="{ on }">
          <v-btn icon v-on="on">
            <v-icon class="icon">mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item v-for="n in 5" :key="n" @click="() => {}">
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "TopNavbar"
};
</script>

<style lang="scss" scoped>
.logo {
  margin-left: 40px;
}
.btnlogo {
  margin-left: 10px;
}
.navbar {
  margin-top: -13px;
  width: 100%;
  position: fixed;
  z-index: 1000;
  font-family: $nav;
}
.search {
  margin-left: 0px;
  @media only screen and (max-width: 768px) {
    margin-left: 50px;
  }
}
.icon{
    @media only screen and (max-width: 768px) {
    margin-left: 0px;
  }
}
</style>