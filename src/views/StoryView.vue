<template>
  <div class="story">
    <v-app-bar elevation="1" color="blue-lighten-1">
      <v-app-bar-title class="ml-8"><router-link to="/">Sui828's portfolio!</router-link></v-app-bar-title>
      <v-spacer />
    </v-app-bar>
    <micomprocedure v-if="path == '/micomprocedure'" />
    <semicolon0103 v-if="path == '/semicolon0103'" />
    <im3py v-if="path == '/im3py'" />
    <portfolio v-if="path == '/portfolio'" />
    <div class="story-bottom">
      <v-btn
        color="white"
        variant="flat"
        prepend-icon="mdi-home"
        to="/"
        >トップに戻る</v-btn
      >
    </div>
  </div>
  <v-footer class="bg-blue-lighten-1">
    <v-col class="text-center my-6" cols="12">
      {{ new Date().getFullYear() }} — sui828
    </v-col>
  </v-footer>
</template>

<script>
import micomprocedure from "../components/Micomprocedure.vue"
import semicolon0103 from "../components/Semicolon0103.vue"
import im3py from "../components/Im3py.vue"
import portfolio from "../components/Portfolio.vue"

export default {
  name: "StoryView",
  components: { micomprocedure, semicolon0103, im3py, portfolio, },
  data: () => ({
    path: "",
  }),
  mounted() {
    this.path = this.$route.path;
  },
};
</script>