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
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/portfolio/portfolio_top.webp"
            alt="トップ画面"
            width="100%"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            ポートフォリオサイトではまず名前を覚えてもらうのが一番だと考えています。そこで、トップにアイコンと名前だけを表示させ、他の情報量をできるだけ少なくできるようシンプルなデザインにしました。
          </p>
        </v-col>
      </div>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "PortfolioView",
};
</script>