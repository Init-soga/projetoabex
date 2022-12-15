<template>
  <v-app>
    <div class="teste">
      <v-card height="80vh" width="60vw" id="container">
        <v-row>
          <v-col cols="6" class="container-esquerda">
            <h1 style="margin-bottom: 8%">Produto X</h1>
            <v-img :src="require('~/assets/arco.svg')" width="13vw" contain />
          </v-col>

          <v-col cols="6" class="container-direita">
            <v-card flat>
              <v-card-text>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores
                natus unde sed consectetur necessitatibus, obcaecati assumenda a
                iste laudantium officia, dolorem, odit error quis et! Obcaecati
                quibusdam distinctio sequi voluptates.
              </v-card-text>
            </v-card>

            <v-expansion-panels accordion flat>
              <v-expansion-panel v-for="(item, i) in 5" :key="i">
                <v-expansion-panel-header
                  >Informação {{ i }}</v-expansion-panel-header
                >
                <v-expansion-panel-content>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  Ut enim ad minim veniam, quis nostrud exercitation ullamco
                  laboris nisi ut aliquip ex ea commodo consequat.
                </v-expansion-panel-content>
              </v-expansion-panel>
            </v-expansion-panels>
          </v-col>
        </v-row>
        <v-row>
          <div class="text-down">
            <v-card flat width="90%">
              <v-card-text>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aut,
                eligendi repellat distinctio nostrum libero ipsum corporis?
                Mollitia suscipit id hic voluptate, excepturi neque ab
                dignissimos, accusantium veritatis soluta quisquam eum nihil!
                Nisi a reprehenderit similique cupiditate, aliquam provident
                quia odit ea praesentium possimus ex, in totam necessitatibus
                iste alias quo quibusdam, sapiente at voluptates eius optio
                accusamus? Tempore rem explicabo culpa facere expedita ipsum
                nisi possimus sit voluptates esse nostrum consectetur,
                blanditiis aliquid? Eveniet enim voluptatem est aliquam error
                necessitatibus mollitia atque cupiditate non minus rerum veniam
                in at repellat modi accusantium itaque, facilis quisquam.
                Fugiat, minus sit eligendi accusantium aliquam sequi laborum
                debitis dolorem, voluptatum doloribus nostrum omnis in deleniti
                nisi quas voluptatem laboriosam eaque officiis commodi magni
                corporis animi ea voluptatibus praesentium. Est commodi rerum,
                natus delectus neque vero voluptate ullam exercitationem, minima
                ipsa ea iste? Nisi voluptates explicabo molestias, vel accusamus
                laudantium praesentium dolorum ea quos saepe.
              </v-card-text>
            </v-card>
          </div>
        </v-row>
      </v-card>
    </div>
  </v-app>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
.teste {
  background-image: url('~/assets/wave.svg');
  display: flex;
  justify-content: center;
}

#container {
  margin-top: 2%;
}

.container-esquerda {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 5%;
}

.container-direita {
  padding-right: 7%;
  padding-top: 3%;
}

.text-down{
    display: flex;
    justify-content: center;
}
</style>
