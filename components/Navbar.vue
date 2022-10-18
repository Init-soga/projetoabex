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
      <v-tab><v-icon></v-icon>A ALDEIA</v-tab>
      <v-tab><v-icon></v-icon>PRODUTOS</v-tab>
      <v-tab><v-icon></v-icon>COMO COMPRAR</v-tab>
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
</style>