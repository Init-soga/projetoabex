<template>
  <v-app>
    <!-- <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row class="content">
          <v-col cols="8" class="texto-card">
            <v-card-title>PASSO 1</v-card-title>
            <v-card-text>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea sequi, at labore quae, officiis distinctio quaerat mollitia, sit id fugiat commodi asperiores ut libero quidem temporibus earum suscipit. Velit labore sunt enim explicabo aperiam magnam, distinctio nisi quidem, aliquid mollitia, itaque fugit molestiae error? Officia, obcaecati? Saepe, consequatur earum eveniet tempore ad accusamus laudantium voluptates repudiandae provident voluptatum, libero, a tenetur alias porro obcaecati excepturi eius molestiae sunt odio error.
              </v-card-text>
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
          <v-col cols="8" class="texto-card">
            <v-card-title>PASSO 2</v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex recusandae nesciunt odio, quae, labore aut debitis ratione iure repudiandae tenetur ipsam sit saepe, consectetur blanditiis eveniet eum corporis cumque. Unde ab placeat rem nulla esse commodi qui error praesentium consequuntur beatae, cumque in sunt vero neque recusandae velit nobis consectetur voluptates! Fugiat veritatis facilis expedita dignissimos fugit, adipisci reiciendis voluptatem cum dolores, beatae eaque vel non? Laudantium impedit commodi expedita?
              </v-card-text>
          </v-col>
        </v-row>
      </v-card>
    </div>
    <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row class="content">
          <v-col cols="8" class="texto-card">
            <v-card-title>PASSO 3</v-card-title>
            <div class="content">
              <v-card-text>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla et molestiae culpa eum minus harum deserunt quam impedit! Perferendis, rerum magni dolorem exercitationem sequi nostrum, quaerat pariatur consequatur dolores sunt nulla cum quo numquam quae enim, delectus laboriosam non. Fugiat dicta molestias ea rerum vero, ipsum accusantium neque? Omnis quia nihil ex, sequi necessitatibus earum eaque enim laborum commodi sit et accusantium facilis sint unde repellat provident eveniet aspernatur! Ipsa?
            </v-card-text>
            </div>
          </v-col>
          <v-col cols="4" class="col-image">
            <div class="user-svg">
              <v-img :src="require('~/assets/PNG/pngegg.png')"></v-img>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div> -->

    <v-stepper v-model="stepper" vertical class="stepper-main">
      <v-stepper-step :complete="stepper > 1" step="1">
        Passo 1
      </v-stepper-step>

      <v-stepper-content step="1">
        <v-card color="grey lighten-1" class="mb-12" height="200px">
          <v-card-title>Descrição do passo 1</v-card-title>
          <v-card-text
            >Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus
            architecto ea accusantium quam, cupiditate doloremque repellat a et
            dolore distinctio eius debitis sit beatae eligendi amet
            exercitationem, voluptate sunt eum illum commodi nam eaque ut! Qui,
            ipsam! Animi nostrum fugiat aut aspernatur molestias quibusdam,
            officia dignissimos iusto in minima placeat libero nulla laudantium
            molestiae at asperiores a culpa delectus fugit porro debitis
            corporis sit. Cumque, pariatur nesciunt excepturi repellat
            consequatur fugiat, est sint eligendi numquam ducimus incidunt nisi
            quo obcaecati saepe distinctio provident inventore possimus in
            alias? Eligendi ipsa expedita et sint eos labore cumque totam
            architecto, eum reprehenderit sapiente?</v-card-text
          >
        </v-card>
        <v-btn color="primary" @click="stepper = 2"> Continue </v-btn>
      </v-stepper-content>

      <v-stepper-step :complete="stepper > 2" step="2">
        Passo 2
      </v-stepper-step>

      <v-stepper-content step="2">
        <v-card color="grey lighten-1" class="mb-12" height="200px">
          <v-card-title>Descrição do passo 2</v-card-title>
          <v-card-text
            >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita
            temporibus non, repellat quod, est culpa maxime natus ratione odio
            illum praesentium rerum delectus, at facere earum. Ut earum beatae
            fugiat culpa similique perspiciatis soluta? Molestias aspernatur ex
            possimus quisquam numquam cum minus blanditiis praesentium et,
            consequatur id eaque voluptatibus, obcaecati temporibus totam
            officia necessitatibus nihil vero! Fugit natus pariatur
            reprehenderit quam excepturi at accusamus ratione maiores, amet
            sapiente labore ipsam ad facilis laboriosam! Adipisci optio
            corporis, modi rem fugiat assumenda ex eius illo repellendus enim
            repellat sed, saepe voluptas ullam sunt consequatur doloremque
            commodi error et hic debitis ab quaerat.</v-card-text
          >
        </v-card>
        <v-btn color="primary" @click="stepper = 3"> Próximo </v-btn>
        <v-btn text @click="stepper--"> Voltar </v-btn>
      </v-stepper-content>

      <v-stepper-step :complete="stepper > 3" step="3">
        Passo 3
      </v-stepper-step>

      <v-stepper-content step="3">
        <v-card color="grey lighten-1" class="mb-12" height="200px"
          ><v-card-title>Descrição do passo 3</v-card-title>
          <v-card-text
            >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita
            temporibus non, repellat quod, est culpa maxime natus ratione odio
            illum praesentium rerum delectus, at facere earum. Ut earum beatae
            fugiat culpa similique perspiciatis soluta? Molestias aspernatur ex
            possimus quisquam numquam cum minus blanditiis praesentium et,
            consequatur id eaque voluptatibus, obcaecati temporibus totam
            officia necessitatibus nihil vero! Fugit natus pariatur
            reprehenderit quam excepturi at accusamus ratione maiores, amet
            sapiente labore ipsam ad facilis laboriosam! Adipisci optio
            corporis, modi rem fugiat assumenda ex eius illo repellendus enim
            repellat sed, saepe voluptas ullam sunt consequatur doloremque
            commodi error et hic debitis ab quaerat.</v-card-text
          >
        </v-card>
        <v-btn color="primary" @click="stepper = 4"> Continue </v-btn>
        <v-btn text @click="stepper--"> Voltar </v-btn>
      </v-stepper-content>

      <v-stepper-step step="4"> Passo 4 </v-stepper-step>
      <v-stepper-content step="4">
        <v-card color="grey lighten-1" class="mb-12" height="200px"
          ><v-card-title>Descrição do passo 2</v-card-title>
          <v-card-text
            >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita
            temporibus non, repellat quod, est culpa maxime natus ratione odio
            illum praesentium rerum delectus, at facere earum. Ut earum beatae
            fugiat culpa similique perspiciatis soluta? Molestias aspernatur ex
            possimus quisquam numquam cum minus blanditiis praesentium et,
            consequatur id eaque voluptatibus, obcaecati temporibus totam
            officia necessitatibus nihil vero! Fugit natus pariatur
            reprehenderit quam excepturi at accusamus ratione maiores, amet
            sapiente labore ipsam ad facilis laboriosam! Adipisci optio
            corporis, modi rem fugiat assumenda ex eius illo repellendus enim
            repellat sed, saepe voluptas ullam sunt consequatur doloremque
            commodi error et hic debitis ab quaerat.</v-card-text
          >
        </v-card>
        <v-btn color="primary" @click="stepper = 1"> Início </v-btn>
        <v-btn text @click="stepper--"> Voltar </v-btn>
      </v-stepper-content>
    </v-stepper>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      stepper: 1,
    }
  },
}
</script>

<style scoped>
.stepper-main {
  margin: 4%;
}
/* .flex-container {
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

.texto-card{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 5%;
} */
</style>
