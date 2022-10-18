<template>
  <div>
    <v-navigation-drawer
      app
    >
    <div id="logo" >
    <v-img :src="logo" />
    </div>
    <v-divider></v-divider>

    <v-tabs vertical>
      <v-tab to="/a-aldeia"><v-icon class="icon-right">mdi-account-group</v-icon>A ALDEIA</v-tab>
      <v-tab to="/produtos"><v-icon class="icon-right">mdi-shopping</v-icon>PRODUTOS</v-tab>
      <v-tab to="/como-comprar"><v-icon class="icon-right">mdi-head-question</v-icon>COMO COMPRAR</v-tab>
    </v-tabs>

    </v-navigation-drawer>

    <v-main>
      <Nuxt />
    </v-main>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        logo: require("~/assets/logo.svg")
      }
    }
  }
</script>

<style scoped>
#logo {
  padding: 5% 8%;
}

.icon-right{
  padding-right: 5%;
}
</style>