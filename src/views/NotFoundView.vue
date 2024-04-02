<template>
  <div class="not-found">
    <v-app-bar flat color="blue-lighten-1">
      <v-app-bar-title>sui828's portfolio!</v-app-bar-title>
      <v-spacer></v-spacer>
      <router-link to="/">
        <v-icon size="large" class="mr-4">mdi-home</v-icon>
      </router-link>
    </v-app-bar>
    <h1>404 not found</h1>
    <p class="my-6">お探しのページは見つかりませんでした。</p>
    <v-btn
      color="blue-lighten-1"
      variant="flat"
      prepend-icon="mdi-home"
      to="/"
      class="mt-10"
      >トップへ戻る</v-btn
    >
  </div>
  <v-footer class="bg-blue-lighten-1">
    <v-col class="text-center mt-6" cols="12">
      {{ new Date().getFullYear() }} — sui828
    </v-col>
  </v-footer>
</template>

<script>
export default {
  name: "NotFoundView",
  data: () => ({}),
};
</script>