<template>
  <div class="story-top">
    <h3>Aioi Aoha's Workshop</h3>
    <v-img
      src="../assets/semicolon0103/aoha_top.webp"
      alt="サイトサムネ画像"
      width="90%"
      max-width="1152"
    ></v-img>
    <v-btn
      color="white"
      variant="flat"
      prepend-icon="mdi-menu-right"
      href="https://semicolon0103.com/"
      target="_blank"
      >サイトへ</v-btn
    >
  </div>
  <div class="story-main">
    <v-row>
      <v-col cols="12">
        <h4>Concept</h4>
      </v-col>
      <v-col cols="12">
        <h5>作品第一</h5>
      </v-col>
      <v-col cols="6" class="px-6">
        <v-img alt="wikiトップ"></v-img>
      </v-col>
      <v-col cols="6" class="px-6">
        <p>
          相生あおはさんからホームページの改修を依頼されたので制作しました。あおはさんは～(紹介文)。そこで、ページを開いた際に活動内容がすぐ見えるようにカルーセルを配置しました。
        </p>
      </v-col>
      <v-col cols="6" class="px-6">
        <p>
          元々自前でホームページを制作なさっていたこともあって、以前のデザインを踏襲しつつモダンなデザインにすることも課題でした。
        </p>
      </v-col>
      <v-col cols="6" class="px-6">
        <v-img alt="wikiトップ"></v-img>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "MicomprocedureView",
  data: () => ({}),
};
</script>