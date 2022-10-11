<template>
  <div>
    <v-toolbar tile flat></v-toolbar>
    <v-navigation-drawer permanent absolute>
      <v-list>
        <v-list-item id="logo">
          <v-img :src="logo"></v-img>
        </v-list-item>
        <v-divider></v-divider>
        <v-tabs vertical>
          <v-tab><v-icon class="icon-tab">mdi-account-group</v-icon><b>A ALDEIA</b></v-tab>
          <v-tab><v-icon class="icon-tab">mdi-shopping</v-icon><b>PRODUTOS</b></v-tab>
          <v-tab><v-icon class="icon-tab">mdi-head-question</v-icon><b>COMO ADQUIRIR</b></v-tab>
        </v-tabs>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      logo: require('~/assets/logo.svg'),
    }
  },
}
</script>

<style lang="scss" scoped>
#logo {
  padding: 8% 5%;
}

.icon-tab{
    padding-right: 5%;
}
</style>
