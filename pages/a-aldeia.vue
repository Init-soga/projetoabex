<template>
  <v-app class="main-wrapper">
    <div class="flex-container">
      <v-card
        width="100vw"
        height="40vh"
        elevation="0"
        style="margin-bottom: 2%; margin-top: ;"
      >
        <v-img
          :src="require('~/assets/handler.jpg')"
          width="100vw"
          height="35vh"
          class="imagem"
        ></v-img>
        <v-card-title
          style="
            font-size: 2em;
            display: flex;
            justify-content: center;
            margin-top: 1.5%;
          "
          >A aldeia</v-card-title
        >
      </v-card>
    </div>

    <div class="flex-container" id="message">
      <v-card width="80vw" height="28vh">
        <v-row class="flex-container">
          <v-col cols="9">
            <v-card-title style="font-size: 1.5em">Artesão X</v-card-title>
            <v-card-text style="font-size: 1em"
              >Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam
              quidem ad deserunt. Similique quos, adipisci alias error minus
              voluptates possimus nulla, tempore esse soluta dolorum labore rem
              aperiam? Iure, voluptate perspiciatis porro libero sunt error
              perferendis aspernatur similique ab odio provident odit, modi
              totam nihil recusandae nisi explicabo id voluptatum tenetur
              distinctio reprehenderit possimus ad? Aut perspiciatis ullam
              asperiores sequi ex necessitatibus praesentium delectus aspernatur
              quis et? Id harum ipsa facilis molestiae perspiciatis, iure,
              ducimus numquam amet dicta totam nulla.
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Magnam delectus magni odio maxime cum voluptatem soluta error veniam earum amet reiciendis, beatae, quos quisquam corporis dicta iure atque, libero dolorum ab laborum. Necessitatibus exercitationem quibusdam, doloribus deleniti assumenda cum aliquid quas aliquam a dicta unde iure velit ipsam illum nam cumque temporibus at iusto dolores eveniet. Architecto delectus itaque atque magni, vitae accusantium culpa quos.
              </v-card-text
            >
          </v-col>
          <v-col cols="3" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/user.svg')"></v-img>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <div class="flex-container" id="message">
      <v-card width="80vw" height="28vh">
        <v-row>
          <v-col cols="3" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/user2.svg')"></v-img>
            </div>
          </v-col>
          <v-col cols="9">
            <v-card-title style="font-size: 1.5em">Artesão Y</v-card-title>
            <v-card-text style="font-size: 1em"
              >Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam
              quidem ad deserunt. Similique quos, adipisci alias error minus
              voluptates possimus nulla, tempore esse soluta dolorum labore rem
              aperiam? Iure, voluptate perspiciatis porro libero sunt error
              perferendis aspernatur similique ab odio provident odit, modi
              totam nihil recusandae nisi explicabo id voluptatum tenetur
              distinctio reprehenderit possimus ad? Aut perspiciatis ullam
              asperiores sequi ex necessitatibus praesentium delectus aspernatur
              quis et? Id harum ipsa facilis molestiae perspiciatis, iure,
              ducimus numquam amet dicta totam nulla.
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Magnam delectus magni odio maxime cum voluptatem soluta error veniam earum amet reiciendis, beatae, quos quisquam corporis dicta iure atque, libero dolorum ab laborum. Necessitatibus exercitationem quibusdam, doloribus deleniti assumenda cum aliquid quas aliquam a dicta unde iure velit ipsam illum nam cumque temporibus at iusto dolores eveniet. Architecto delectus itaque atque magni, vitae accusantium culpa quos.
              </v-card-text
            >
          </v-col>
        </v-row>
      </v-card>
    </div>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
    }
  },
  methods: {},
}
</script>

<style scoped>
.flex-container {
  display: flex;
  justify-content: center;

}

#message {
  margin-top: 1.5%;
}

.user-svg {
  width: 150px;
}

.col-image {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
