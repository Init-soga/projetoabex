<template>
  <div>
    <v-container style="margin-top: 2%">
      <v-row v-for="number in 3" :key="number" class="linha-produtos">
        <v-col cols="3">
          <v-card height="30vh">
            <v-row>
              <v-col cols="12" class="container-produto">
                <div class="imagem-produto">
                  <v-img :src="arrayProdutos[imagemEscolhida]">
                  </v-img>
                </div>
              </v-col>
            </v-row>
            <v-row class="titulo-produto">
              <h3>Produto A</h3>
            </v-row>
            <v-row class="titulo-produto">
              <p>R$ XX,XX</p>
            </v-row>
            <v-row class="titulo-produto">
              <v-btn style="margin: 5%">Ver mais!</v-btn>
            </v-row>
          </v-card>
        </v-col>
        <v-spacer></v-spacer>
        <v-col cols="3">
          <v-card height="30vh">
            <v-row>
              <v-col cols="12" class="container-produto">
                <div class="imagem-produto">
                  <v-img :src="require('~/assets/compras/produto2.svg')">
                  </v-img>
                </div>
              </v-col>
            </v-row>
            <v-row class="titulo-produto">
              <h3>Produto B</h3>
            </v-row>
            <v-row class="titulo-produto">
              <p>R$ XX,XX</p>
            </v-row>
            <v-row class="titulo-produto">
              <v-btn style="margin: 5%">Ver mais!</v-btn>
            </v-row>
          </v-card>
        </v-col>
        <v-spacer></v-spacer
        ><v-col cols="3">
          <v-card height="30vh">
            <v-row>
              <v-col cols="12" class="container-produto">
                <div class="imagem-produto">
                  <v-img :src="require('~/assets/compras/produto3.svg')">
                  </v-img>
                </div>
              </v-col>
            </v-row>
            <v-row class="titulo-produto">
              <h3>Produto C</h3>
            </v-row>
            <v-row class="titulo-produto">
              <p>R$ XX,XX</p>
            </v-row>
            <v-row class="titulo-produto">
              <v-btn style="margin: 5%">Ver mais!</v-btn>
            </v-row>
          </v-card>
        </v-col>
        <v-spacer></v-spacer>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      arrayProdutos: ["/assets/compras/produto3.svg", "/assets/compras/produto2.svg", "/assets/compras/produto1.svg", "/assets/compras/produto4.svg"],
    }
  },
  methods: {
    randomImagePicker(){
      let choosen = Math.floor(Math.random() * this.arrayProdutos.length);
      this.imagemEscolhida = choosen;
    }
  },
  created(){
    this.randomImagePicker();
  }
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

.linha-produtos{
  margin-bottom: 2%;
}
</style>
