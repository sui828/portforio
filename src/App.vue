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
    path: "top",
    path_old: "",
  }),

  methods: {
    setRamune() {
      this.path = this.$route.name;
    },
  },

  watch: {
    $route(newRoute, oldRoute) {
      const topPath = newRoute.name;
      const oldPath = oldRoute.name;
      this.path = topPath;
      console.log(this.path);
      this.path_old = oldPath;
    },
  },
};
</script>

<style>
@import "./assets/stylesheet.css";
</style>
