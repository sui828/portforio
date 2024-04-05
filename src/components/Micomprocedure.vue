<template>
  <div class="story-top">
    <h3>Micomprocedure</h3>
    <v-img
      src="../assets/micomprocedure/proc_top.webp"
      alt="サイトサムネ画像"
      width="90%"
      max-width="1152"
    ></v-img>
    <v-btn
      color="white"
      variant="flat"
      prepend-icon="mdi-menu-right"
      href="https://micomprocedure.com/"
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
        <h5>見栄えよく、引き継ぎやすく</h5>
      </v-col>
      <div class="d-sm-flex">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/micomprocedure/proc_1.webp"
            alt="wikiトップ"
            width="100%"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            現在、Micomprocedureというゲーム制作サークルに在籍しています。学部2年生のときにそのサークルの副部長になり、私が主体となり新しいホームページを作ることになりました。<br />サークルには以前からWikiの形で活動報告やサークルで制作したものの紹介などを行っていました。しかし、長年使われていたため更新はできるものの保守ができる人がおらず、SSL証明書の有効期限が切れた際にそれが置いてある階層はおろかWiki本体が置いてある階層も分からずに困惑した記憶があります。
          </p>
        </v-col>
      </div>
      <div class="d-sm-flex flex-row-reverse">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/micomprocedure/proc_2.webp"
            alt="作品ページ"
            width="100%"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            デザインは当時の部長にお願いして、私は実装を担当しました。実装する際に実装のしやすさ、初学のハードルの低さからVue.jsを勉強しながら使っていくことにしました。更新がしやすいように雛形の部分とデータの部分を分離させ、データを変えるだけで更新作業が終わるようになったのが大きいと感じています。今後はVueのバージョンアップ作業とタスクフローの引き継ぎが課題です。
          </p>
        </v-col>
      </div>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "MicomprocedureView",
};
</script>