<template>
  <v-app>
    <v-app-bar class="superior-navbar">
      <div class="flex-container">
        <v-img :src="logo" width="45" />
      </div>
      <div style="margin-left: 1%;">
        <h2>Kamé-Kanhru</h2>
      </div>
      <v-spacer></v-spacer>
      <v-btn link nuxt to="/a-aldeia" text style="margin-right: 0.5%;"
        ><v-icon class="icon-right">mdi-account-group</v-icon>A ALDEIA</v-btn
      > 
      <v-btn link nuxt to="/produtos" text  style="margin-right: 0.5%;"
        ><v-icon class="icon-right">mdi-shopping</v-icon>PRODUTOS</v-btn
      >
      <v-btn link nuxt to="/como-comprar" text
        ><v-icon class="icon-right">mdi-head-question</v-icon>COMO
        COMPRAR</v-btn
      >
    </v-app-bar>
    <v-main>
      <Nuxt />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Toolbar from './Toolbar.vue'
export default {
  components: { Toolbar },
  data() {
    return {
      logo: require('/assets/compras/produto1.svg'),
    }
  },
}
</script>

<style scoped>

#logo {
  padding: 5% 8%;
}

.icon-right {
  padding-right: 5%;
}

.flex-container {
  display: flex;
  flex-direction: row;
  align-items: center;
}
</style>
