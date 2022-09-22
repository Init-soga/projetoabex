<template>
  <div>
    <v-footer padless fixed>
      <v-col cols="12">
        <div class="footerComponent"> 
        {{new Date().getFullYear()}} - <b>Kame-Kunhru</b>
        </div>
      </v-col>
    </v-footer>
  </div>
</template>

<script>
export default {
    name: "FooterComponent"
}
</script>

<style lang="scss" scoped>
* {
    background-color: #472D2D;
}

.footerComponent{
    display: flex;
    justify-content: center;
}
</style>
