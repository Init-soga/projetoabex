<template>
  <div>
    <v-footer fixed inset app>
        <v-row>
          <v-col cols="12" class="fab-btn">
            <v-btn text fab><v-icon>mdi-facebook</v-icon></v-btn>
            <v-btn text fab><v-icon>mdi-instagram</v-icon></v-btn>
            <v-btn text fab><v-icon>mdi-twitter</v-icon></v-btn>
          </v-col>
        </v-row>
    </v-footer>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style lang="scss" scoped>
.fab-btn{
  display: flex;
  justify-content: center;
}
</style>
