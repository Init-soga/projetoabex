<template>
  <div class="mainLayout">
    <v-app-bar color="#F7E9D7">
      <v-btn text nuxt to="/" depressed>Kame-Kunhru</v-btn>
      <v-spacer></v-spacer>
      <v-btn text nuxt to="/como-comprar">Quem somos</v-btn>
      <v-btn text>Como comprar</v-btn>
    </v-app-bar>
    <Nuxt />
    <div class="footer">
    <FooterComponent />
    </div>
  </div>
</template>

<script>
import FooterComponent from "../components/footer.vue"
export default {
  data(){
    return{}
  },
  components: {
    FooterComponent
  }
}
</script>

<style lang="scss" scoped>
.mainLayout{
  background-color: #EBD8C3;
  min-height: 100vh;
  height: 100%;
}

</style>
