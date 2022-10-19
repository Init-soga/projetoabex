<template>
  <div>
    <div class="flex-container">
      <v-card width="75vw" height="100%" style="margin-top: 2%;">
        <v-card-title>A aldeia</v-card-title>
        <v-card-text
          >Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam iure
          facilis, eius sunt hic excepturi, aspernatur pariatur cumque
          consectetur rerum ducimus labore. Laudantium, dolores hic pariatur
          aliquam ad dolor numquam suscipit deleniti! Deserunt dolores veniam ex
          iure, ducimus perferendis omnis similique tempore vero expedita.
          Adipisci possimus cupiditate expedita corporis. Sint, ipsa a minima
          illum impedit veniam, quae, debitis quibusdam repellat quas doloribus!
          Fuga vitae, ut veniam repudiandae sit numquam ad ducimus modi
          temporibus, labore eum tempora excepturi voluptates quisquam ex
          asperiores et! Expedita veniam aspernatur excepturi perferendis porro
          blanditiis, voluptates rem quaerat omnis sint inventore ut deleniti
          dolores, quo, debitis est voluptatibus molestias! Pariatur, inventore
          fuga nobis labore consectetur assumenda dolorem unde doloribus non
          molestiae aliquam, odio nam rerum blanditiis ullam reprehenderit
          asperiores id iste necessitatibus libero in porro ipsa! Hic quas dicta
          nemo vitae magni! Quisquam porro excepturi necessitatibus provident
          iste, quibusdam nulla sequi hic eos amet velit a consequuntur est eum
          aperiam ipsa maiores magni adipisci deserunt quo. Perspiciatis nostrum
          qui, vero sit exercitationem reiciendis veniam in eveniet, aliquam
          asperiores esse! Eos expedita odit deleniti eaque et, quibusdam,
          cupiditate tempore exercitationem qui harum accusamus autem
          consectetur saepe neque facere? Libero, doloribus odit. Labore illo
          eos repellendus, aliquid magni pariatur quaerat obcaecati excepturi
          voluptatem, consequatur sint sed veritatis unde assumenda modi
          dignissimos ipsam quisquam error porro. Quo, omnis numquam quisquam
          vel cum officiis tempora excepturi, sequi fugit dolore odio! Tempora
          at nesciunt iure dolor, iste similique officiis perspiciatis, iusto
          nam deserunt nisi dolores alias. Unde maiores, dolorum itaque magnam
          nihil aliquam quibusdam obcaecati harum vitae voluptatum, reiciendis
          placeat animi mollitia odio corrupti quod aperiam rerum. Temporibus
          quas accusamus ea repellendus, dolorum possimus adipisci magnam
          repudiandae corporis dignissimos quo harum non sint? Ipsam illum
          possimus, nostrum deserunt velit quas non error quasi aliquid
          excepturi pariatur quos temporibus voluptatibus a
          dolorem?</v-card-text
        >
      </v-card>
    </div>

    <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row>
          <v-col cols="8">
            <v-card-title>Artesão X</v-card-title>
            <v-card-text>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam quidem ad deserunt. Similique quos, adipisci alias error minus voluptates possimus nulla, tempore esse soluta dolorum labore rem aperiam? Iure, voluptate perspiciatis porro libero sunt error perferendis aspernatur similique ab odio provident odit, modi totam nihil recusandae nisi explicabo id voluptatum tenetur distinctio reprehenderit possimus ad? Aut perspiciatis ullam asperiores sequi ex necessitatibus praesentium delectus aspernatur quis et? Id harum ipsa facilis molestiae perspiciatis, iure, ducimus numquam amet dicta totam nulla.</v-card-text>
          </v-col>
          <v-col cols="4" class="col-image">
            <div class="user-svg">
            <v-img :src="require('~/assets/user.svg')"></v-img>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <div class="flex-container" id="message">
      <v-card width="75vw" height="100%">
        <v-row>
           <v-col cols="4" class="col-image">
            <div class="user-svg">
            <v-img :src="require('~/assets/user2.svg')"></v-img>
            </div>
          </v-col>
          <v-col cols="8">
            <v-card-title>Artesão Y</v-card-title>
            <v-card-text>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quam quidem ad deserunt. Similique quos, adipisci alias error minus voluptates possimus nulla, tempore esse soluta dolorum labore rem aperiam? Iure, voluptate perspiciatis porro libero sunt error perferendis aspernatur similique ab odio provident odit, modi totam nihil recusandae nisi explicabo id voluptatum tenetur distinctio reprehenderit possimus ad? Aut perspiciatis ullam asperiores sequi ex necessitatibus praesentium delectus aspernatur quis et? Id harum ipsa facilis molestiae perspiciatis, iure, ducimus numquam amet dicta totam nulla.</v-card-text>
          </v-col>
        </v-row>
      </v-card>
    </div>

  </div>
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

#message{
  margin-top: 2%;
}

.user-svg{
  width: 150px;
}

.col-image{
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
