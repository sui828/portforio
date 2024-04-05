<template>
  <div class="story-top">
    <h3 style="font-family: 'BIZ UDPGothic', sans-serif">生成物置き場</h3>
    <v-img
      src="../assets/im3py/im3py_top.webp"
      alt="サイトサムネ画像"
      width="90%"
      max-width="1152"
    ></v-img>
    <v-row>
      <v-col
        cols="12"
        sm="6"
        md="6"
        lg="6"
        xl="6"
        class="d-flex justify-center"
      >
        <v-btn
          color="white"
          variant="flat"
          prepend-icon="mdi-menu-right"
          href="https://sui828.github.io/"
          target="_blank"
          width="120"
          class="mt-3"
          >サイトへ</v-btn
        >
      </v-col>
      <v-col
        cols="12"
        sm="6"
        md="6"
        lg="6"
        xl="6"
        class="d-flex justify-center"
      >
        <v-btn
          color="white"
          variant="flat"
          prepend-icon="mdi-menu-right"
          href="https://github.com/sui828/sui828.github.io"
          target="_blank"
          width="120"
          class="mt-3"
          >GitHub</v-btn
        >
      </v-col>
    </v-row>
  </div>
  <div class="story-main">
    <v-row>
      <v-col cols="12">
        <h4>Concept</h4>
      </v-col>
      <v-col cols="12">
        <h5>見栄えに特化する</h5>
      </v-col>
      <div class="d-sm-flex">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/im3py/im3py_1.webp"
            alt="wikiトップ"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p>
            大学に入ってから、創作系のサークルに複数入って各所で創作活動をしています。作品をまとめておく場所が欲しかったので今できることを使って制作してみました。自分だけが見ることができれば良いというモチベーションの下で、使い勝手や視認性より見栄えの良さに力を注ぎたく思いデザインしました。
          </p>
        </v-col>
      </div>
      <div class="d-sm-flex flex-row-reverse">
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <v-img
            src="../assets/im3py/im3py_2.webp"
            alt="作品ページ"
          />
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="6" xl="6" class="px-4 py-8 d-flex align-center">
          <p class="pb-12">
            スマートフォンでは右上の星座マークボタンから各ページに飛べるようにしました。星座の画像に合わせてボタンの位置を細かく調整しています。
          </p>
        </v-col>
      </div>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "Im3pyView",
};
</script>