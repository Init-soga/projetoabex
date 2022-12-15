<template>
  <div class="teste">
    <v-container style="padding-top: 2%;">
      <div>
        <v-row v-for="number in 3" :key="number" class="linha-produtos">
          <v-col cols="3">
            <v-card height="30vh" elevation="4">
              <v-row>
                <v-col cols="12" class="container-produto">
                  <div class="imagem-produto">
                    <v-img :src="require('~/assets/compras/produto1.svg')">
                    </v-img>
                  </div>
                </v-col>
              </v-row>
              <v-row class="titulo-produto">
                <h3>Produto X</h3>
              </v-row>
              <v-row class="titulo-produto">
                <p>R$ XX,XX</p>
              </v-row>
              <v-row class="titulo-produto">
                <v-btn style="margin: 5%" text>Ver mais!</v-btn>
              </v-row>
            </v-card>
          </v-col>
          <v-spacer></v-spacer>
          <v-col cols="3">
            <v-card height="30vh" elevation="4">
              <v-row>
                <v-col cols="12" class="container-produto">
                  <div class="imagem-produto">
                    <v-img :src="require('~/assets/compras/produto2.svg')">
                    </v-img>
                  </div>
                </v-col>
              </v-row>
              <v-row class="titulo-produto">
                <h3>Produto X</h3>
              </v-row>
              <v-row class="titulo-produto">
                <p>R$ XX,XX</p>
              </v-row>
              <v-row class="titulo-produto">
                <v-btn style="margin: 5%" text>Ver mais!</v-btn>
              </v-row>
            </v-card>
          </v-col>
          <v-spacer></v-spacer
          ><v-col cols="3">
            <v-card height="30vh" elevation="4">
              <v-row>
                <v-col cols="12" class="container-produto">
                  <div class="imagem-produto">
                    <v-img :src="require('~/assets/compras/produto3.svg')">
                    </v-img>
                  </div>
                </v-col>
              </v-row>
              <v-row class="titulo-produto">
                <h3>Produto X</h3>
              </v-row>
              <v-row class="titulo-produto">
                <p>R$ XX,XX</p>
              </v-row>
              <v-row class="titulo-produto">
                <v-btn style="margin: 5%" text>Ver mais!</v-btn>
              </v-row>
            </v-card>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arrayProdutos: [
        '/assets/compras/produto3.svg',
        '/assets/compras/produto2.svg',
        '/assets/compras/produto1.svg',
        '/assets/compras/produto4.svg',
      ],
    }
  },
  components: {},
  methods: {
    randomImagePicker() {
      let choosen = Math.floor(Math.random() * this.arrayProdutos.length)
      this.imagemEscolhida = choosen
    },
  },
  created() {
    this.randomImagePicker()
  },
}
</script>

<style lang="scss" scoped>
.imagem-produto {
  width: 120px;
}

.container-produto {
  display: flex;
  justify-content: center;
  align-items: center;
}

.titulo-produto {
  display: flex;
  justify-content: center;
}

.linha-produtos {
  margin-bottom: 2%;
}

.teste {
  background-image: url('~/assets/wave.svg');
}
</style>
