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
        <h5>作品を印象付ける</h5>
      </v-col>
      <div class="d-sm-flex">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/semicolon0103/aoha_1.webp"
            alt="ブログトップ"
            width="100%"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            同じサークルに所属していた相生あおはさんからホームページの改修を依頼されて制作しました。あおはさんはコンポーザーということもあって、ページを開いた際に活動内容がすぐ見えるよう一番上にカルーセルを配置しました。他にブログを執筆されたり旅行されたりしており、その情報の重要度が同じくらい高いということで、カルーセルにはそちらの情報も含めています。
          </p>
        </v-col>
      </div>
      <div class="d-sm-flex flex-row-reverse">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/semicolon0103/aoha_2.webp"
            alt="曲紹介ページ"
            width="100%"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            元々自前でホームページを作成されていたこともあり、内容や細かいレイアウトはそこから大きい変更がないようにしています。その中で、曲紹介ページでは雛形となるコンポーネントを作成し、更新作業を大幅に効率化できました。
          </p>
        </v-col>
      </div>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "SemicolonView",
};
</script>