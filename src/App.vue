<template>
  <v-app>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    ramune: "top",
    page: "",
  }),

  methods: {
    setRamune() {
      this.ramune = this.$route.name;
    },
  },

  watch: {
    // Pathの変化: Page移動を監視する
    $route(newRoute, oldRoute) {
      const topPath = newRoute.name;
      const oldPath = oldRoute.name;
      this.ramune = topPath;
      console.log(this.ramune);
      this.page = oldPath;
    },
  },
};
</script>

<style>
@import "./assets/stylesheet.css";
</style>
