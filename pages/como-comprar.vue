<template>
  <div>
    <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row class="contente">
          <v-col cols="8">
            <v-card-title>Carrinho De Compras</v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam
              quidem ad deserunt. Similique quos, adipisci alias error minus
              voluptates possimus nulla, tempore esse soluta dolorum labore rem
              aperiam? Iure, voluptate perspiciatis porro libero sunt error
              perferendis aspernatur similique ab odio provident odit, modi
              totam nihil recusandae nisi explicabo id voluptatum tenetur
              distinctio reprehenderit possimus ad? Aut perspiciatis ullam
              asperiores sequi ex necessitatibus praesentium delectus aspernatur
              quis et? Id harum ipsa facilis molestiae perspiciatis, iure,
              ducimus numquam amet dicta totam nulla.</v-card-text
            >
            <br />
            <v-btn style="margin: 5%">Ver mais!</v-btn>
          </v-col>
          <v-col cols="4" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/PNG/pngegg.png')"></v-img>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <div class="flex-container">
      <v-card width="75vw" height="100%">
        <v-row>
          <v-col cols="4" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/PNG/handshake icon.png')"></v-img>
            </div>
          </v-col>
          <v-col cols="8">
            <v-card-title>Após Comprar</v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam
              quidem ad deserunt. Similique quos, adipisci alias error minus
              voluptates possimus nulla, tempore esse soluta dolorum labore rem
              aperiam? Iure, voluptate perspiciatis porro libero sunt error
              perferendis aspernatur similique ab odio provident odit, modi
              totam nihil recusandae nisi explicabo id voluptatum tenetur
              distinctio reprehenderit possimus ad? Aut perspiciatis ullam
              asperiores sequi ex necessitatibus praesentium delectus aspernatur
              quis et? Id harum ipsa facilis molestiae perspiciatis, iure,
              ducimus numquam amet dicta totam nulla.</v-card-text
            >
            <v-btn style="margin: 5%">Ver mais!</v-btn>
          </v-col>
        </v-row>
      </v-card>
    </div>
    <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row class="contente">
          <v-col cols="8">
            <v-card-title>Carrinho De Compras</v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam
              quidem ad deserunt. Similique quos, adipisci alias error minus
              voluptates possimus nulla, tempore esse soluta dolorum labore rem
              aperiam? Iure, voluptate perspiciatis porro libero sunt error
              perferendis aspernatur similique ab odio provident odit, modi
              totam nihil recusandae nisi explicabo id voluptatum tenetur
              distinctio reprehenderit possimus ad? Aut perspiciatis ullam
              asperiores sequi ex necessitatibus praesentium delectus aspernatur
              quis et? Id harum ipsa facilis molestiae perspiciatis, iure,
              ducimus numquam amet dicta totam nulla.
            </v-card-text>
            <br />
            <v-btn style="margin: 5%">Ver mais!</v-btn>
          </v-col>
          <v-col cols="4" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/PNG/pngegg.png')"></v-img>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
* {
  text-align: justify;
}

.flex-container {
  display: flex;
  justify-content: center;
  margin-bottom: 2%;
}
.contente {
  padding: 5%;
}

.user-svg {
  width: 300px;
}
#message {
  margin-top: 2%;
}
.col-image {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
