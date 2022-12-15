<template>
  <v-app>
    <div class="teste">
      <div class="titulo">
        <h1>Como adquirir nossos produtos?</h1>
      </div>

      <v-stepper v-model="stepper" vertical class="stepper-main">
        <v-stepper-step :complete="stepper > 1" step="1" color="#DAB88B">
          <h3>Passo 1</h3>
        </v-stepper-step>

        <v-stepper-content step="1">
          <v-card class="mb-12" height="100%" elevation="0">
            <v-card-title>Descrição do passo 1</v-card-title>
            <v-card-text
             style="font-size: 1.1em;" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus
              architecto ea accusantium quam, cupiditate doloremque repellat a
              et dolore distinctio eius debitis sit beatae eligendi amet
              exercitationem, voluptate sunt eum illum commodi nam eaque ut!
              Qui, ipsam! Animi nostrum fugiat aut aspernatur molestias
              quibusdam, officia dignissimos iusto in minima placeat libero
              nulla laudantium molestiae at asperiores a culpa delectus fugit
              porro debitis corporis sit. Cumque, pariatur nesciunt excepturi
              repellat consequatur fugiat, est sint eligendi numquam ducimus
              incidunt nisi quo obcaecati saepe distinctio provident inventore
              possimus in alias? Eligendi ipsa expedita et sint eos labore
              cumque totam architecto, eum reprehenderit sapiente?</v-card-text
            >
          </v-card>
          <v-btn color="#DAB88B" @click="stepper = 2" dark> Próximo </v-btn>
        </v-stepper-content>

        <v-stepper-step :complete="stepper > 2" step="2" color="#DAB88B">
          <h3>Passo 2</h3>
        </v-stepper-step>

        <v-stepper-content step="2">
          <v-card color="" class="mb-12" height="100%" elevation="0">
            <v-card-title>Descrição do passo 2</v-card-title>
            <v-card-text style="font-size: 1.1em;"
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit.
              Expedita temporibus non, repellat quod, est culpa maxime natus
              ratione odio illum praesentium rerum delectus, at facere earum. Ut
              earum beatae fugiat culpa similique perspiciatis soluta? Molestias
              aspernatur ex possimus quisquam numquam cum minus blanditiis
              praesentium et, consequatur id eaque voluptatibus, obcaecati
              temporibus totam officia necessitatibus nihil vero! Fugit natus
              pariatur reprehenderit quam excepturi at accusamus ratione
              maiores, amet sapiente labore ipsam ad facilis laboriosam!
              Adipisci optio corporis, modi rem fugiat assumenda ex eius illo
              repellendus enim repellat sed, saepe voluptas ullam sunt
              consequatur doloremque commodi error et hic debitis ab
              quaerat.</v-card-text
            >
          </v-card>
          <v-btn color="#DAB88B" @click="stepper = 3" dark> Próximo </v-btn>
          <v-btn text @click="stepper--"> Voltar </v-btn>
        </v-stepper-content>

        <v-stepper-step :complete="stepper > 3" step="3" color="#DAB88B">
          <h3>Passo 3</h3>
        </v-stepper-step>

        <v-stepper-content step="3">
          <v-card color="" class="mb-12" height="100%" elevation="0"
            ><v-card-title>Descrição do passo 3</v-card-title>
            <v-card-text style="font-size: 1.1em;"
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit.
              Expedita temporibus non, repellat quod, est culpa maxime natus
              ratione odio illum praesentium rerum delectus, at facere earum. Ut
              earum beatae fugiat culpa similique perspiciatis soluta? Molestias
              aspernatur ex possimus quisquam numquam cum minus blanditiis
              praesentium et, consequatur id eaque voluptatibus, obcaecati
              temporibus totam officia necessitatibus nihil vero! Fugit natus
              pariatur reprehenderit quam excepturi at accusamus ratione
              maiores, amet sapiente labore ipsam ad facilis laboriosam!
              Adipisci optio corporis, modi rem fugiat assumenda ex eius illo
              repellendus enim repellat sed, saepe voluptas ullam sunt
              consequatur doloremque commodi error et hic debitis ab
              quaerat.</v-card-text
            >
          </v-card>
          <v-btn color="#DAB88B" @click="stepper = 4"> Próximo </v-btn> 
          <v-btn text @click="stepper--"> Voltar </v-btn>
        </v-stepper-content>

        <v-stepper-step step="4" color="#DAB88B">
          <h3>Passo 4</h3>
        </v-stepper-step>
        <v-stepper-content step="4">
          <v-card color="" class="mb-12" height="100%" elevation="0"
            ><v-card-title>Descrição do passo 2</v-card-title>
            <v-card-text style="font-size: 1.1em;"
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit.s
              Expedita temporibus non, repellat quod, est culpa maxime natus
              ratione odio illum praesentium rerum delectus, at facere earum. Ut
              earum beatae fugiat culpa similique perspiciatis soluta? Molestias
              aspernatur ex possimus quisquam numquam cum minus blanditiis
              praesentium et, consequatur id eaque voluptatibus, obcaecati
              temporibus totam officia necessitatibus nihil vero! Fugit natus
              pariatur reprehenderit quam excepturi at accusamus ratione
              maiores, amet sapiente labore ipsam ad facilis laboriosam!
              Adipisci optio corporis, modi rem fugiat assumenda ex eius illo
              repellendus enim repellat sed, saepe voluptas ullam sunt
              consequatur doloremque commodi error et hic debitis ab
              quaerat.</v-card-text
            >
          </v-card>
          <v-btn color="#DAB88B" @click="stepper = 1" dark> Início </v-btn>
          <v-btn text @click="stepper--"> Voltar </v-btn>
        </v-stepper-content>
      </v-stepper>
    </div>
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
  margin-top: 0;
}

.titulo {
  display: flex;
  justify-content: center;
  margin: 1.5% 0;
}

.teste {
  background-image: url('~/assets/wave.svg');
}
</style>
