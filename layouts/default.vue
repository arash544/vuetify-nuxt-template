<template>
  <div>
    <v-content>
      <v-container>
        <Nav/>
        <nuxt />
      </v-container>
    </v-content>
    </div>
</template>

<script>
import Nav from '@/components/navbar-part/Nav'
export default {
  components:{
    Nav
  }
}
</script>
<style land="scss">
:root{
  --primary:rgb(100, 1, 158);
}
</style>
