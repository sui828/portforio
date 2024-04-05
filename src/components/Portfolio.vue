<template>
  <div class="story-top">
    <h3 style="font-family: 'BIZ UDPGothic', sans-serif;">ポートフォリオ</h3>
    <v-img
      src="../assets/portfolio/portfolio_top.webp"
      alt="サイトサムネ画像"
      width="90%"
      max-width="1152"
    ></v-img>
    <v-btn
      color="white"
      variant="flat"
      prepend-icon="mdi-menu-right"
      href="https://github.com/sui828/portforio"
      target="_blank"
      >GitHub</v-btn
    >
  </div>
  <div class="story-main">
    <v-row>
      <v-col cols="12">
        <h4>Concept</h4>
      </v-col>
      <v-col cols="12">
        <h5>情報量を減らす</h5>
      </v-col>
      <div class="d-sm-flex">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8">
          <v-img alt="wikiトップ"></v-img>
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8">
          <p>
            現在、Micomprocedureというゲーム制作サークルに在籍しています。学部2年生のときにそのサークルの副部長になり、私が主体となり新しいホームページを作ることになりました。<br />サークルには以前からWikiの形で活動報告やサークルで制作したものの紹介などを行っていました。しかし、長年使われていたため、更新はできるものの保守ができる人がおらず、SSL証明書の有効期限が切れた際にそれが置いてある階層はおろかWiki本体が置いてある階層も分からず、てんやわんやになりながらなんとか乗り越えた記憶があります。そこで、サーバも新調してサイトも新しく作ろうという話が上がりました。
          </p>
        </v-col>
      </div>
      <div class="d-sm-flex flex-row-reverse">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8">
          <v-img
            src="../assets/micomprocedure/proc_top.webp"
            alt="wikiトップ"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8">
          <p>
            デザインは当時の部長にお願いして、私は実装を担当しました。実装する際に実装のしやすさ、初学のハードルの低さからVue.jsを勉強しながら使っていくことにしました。
          </p>
        </v-col>
      </div>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "MicomprocedureView",
  data: () => ({}),
};
</script>