<template>
  <div>
    <v-container class="container" app>
      <v-row no-gutters>
        <v-col v-for="n in 3" :key="n">
          <v-card class="cardProduto">{{n}}</v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data(){
    return{
      
    }
  }
}
</script>

<style lang="scss" scoped>
.mainLayout > div:nth-child(2){
  margin: 2%;
}

.cardProduto{
  margin: 2%;
  height: 20vh;
  
}
</style>
