<template>
  <div>
    <v-app-bar class="superior-navbar" app color="#f5f5f5" flat>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer
      app
      v-model="drawer"
    >
    <div id="logo" >
    <v-img :src="logo" />
    </div>

    <v-tabs vertical>
      <v-tab to="/a-aldeia"><v-icon class="icon-right">mdi-account-group</v-icon>A ALDEIA</v-tab>
      <v-tab to="/produtos"><v-icon class="icon-right">mdi-shopping</v-icon>PRODUTOS</v-tab>
      <v-tab to="/como-comprar"><v-icon class="icon-right">mdi-head-question</v-icon>COMO COMPRAR</v-tab>
    </v-tabs>

    </v-navigation-drawer>

    <v-main>
      <Nuxt />
      <Footer />
    </v-main>
  </div>
</template>

<script>
import Toolbar from './Toolbar.vue'
  export default {
  components: { Toolbar },
    data(){
      return{
        logo: require("~/assets/logo.svg"),
        drawer: false
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