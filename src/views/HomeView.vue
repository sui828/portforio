<template>
  <v-navigation-drawer v-model="drawer" location="right"> </v-navigation-drawer>
  <v-icon size="60" color="blue-lighten-1" @click="drawer = !drawer" class="drawer">mdi-menu</v-icon>
  <div class="top">
    <div class="top-icon">
      <v-img
        src="../assets/icon.webp"
        alt="sui828's icon"
        width="60%"
        aspect-ratio="1"
      ></v-img>
      <div class="name-box">Sui828's portfolio!</div>
    </div>
    <div class="arrow">
      <v-icon size="100">mdi-chevron-double-down</v-icon>
      <p>scroll</p>
    </div>
  </div>
  <div class="banner"><h1>About</h1></div>
  <div class="about">
    <v-row>
      <v-col cols="12">
        <h2>Profile</h2>
        <div class="about-box">
          <p>
            2001年生まれ。現在、東北大学大学院理学研究科所属。専攻は数学(解析学/偏微分方程式論)。<br />2022年、サークルでWebページを制作したことをきっかけにしてVue.jsの勉強を独学で始める。
          </p>
        </div>
      </v-col>
      <v-col cols="12">
        <h2>Social Media</h2>
        <div class="about-box">
          <a href="https://twitter.com/828sui" target="_blank">
            <v-icon>mdi-twitter</v-icon>
          </a>
          <a href="https://github.com/sui828" target="_blank">
            <v-icon>mdi-github</v-icon>
          </a>
        </div>
      </v-col>
      <v-col cols="12">
        <h2>Skills</h2>
        <div class="about-box">
          <p>
            - HTML<br />- CSS<br />- JavaScript<br />- Vue.js<br />- C#<br />-
            Unity
          </p>
        </div>
      </v-col>
    </v-row>
  </div>
  <div class="banner"><h1>Works</h1></div>
  <div class="works">
    <v-row>
      <v-col cols="6" md="4" lg="4" xl="3" v-for="i in works" :key="i">
        <v-card variant="outlined" color="blue-lighten-4">
          <v-img :src="i.src" class="mb-4"></v-img>
          <v-card-subtitle class="d-flex">
            <v-chip
              v-for="c in i.tag"
              :key="c"
              flat
              :color="c.color"
              :prepend-icon="c.icon"
              class="mr-1"
              >{{ c.text }}</v-chip
            >
          </v-card-subtitle>
          <v-card-title class="mx-3 text-blue-lighten-1 pt-5">{{
            i.title
          }}</v-card-title>
          <v-row class="mb-6">
            <v-col cols="6">
              <v-btn
                color="blue-lighten-1"
                variant="flat"
                prepend-icon="mdi-menu-right"
                :href="i.to"
                target="_blank"
                >サイトへ</v-btn
              >
            </v-col>
            <v-col cols="6">
              <v-btn
                color="blue-lighten-1"
                variant="flat"
                prepend-icon="mdi-menu-right"
                :to="i.id"
                >制作小話</v-btn
              >
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </div>
  <v-footer class="bg-blue-lighten-1">
    <v-col class="text-center my-6" cols="12">
      {{ new Date().getFullYear() }} — sui828
    </v-col>
  </v-footer>
</template>

<script>
export default {
  name: "HomeView",
  data: function () {
    return {
      drawer: false,
      page: "",
      works: [
        {
          id: "micomprocedure",
          src: require("../assets/micomprocedure/proc_ico.webp"),
          to: "https://micomprocedure.com/",
          title: "Micomprocedure",
          tag: [
            { icon: "mdi-vuejs", text: "Vue 2", color: "#3c4f64" },
            { icon: "mdi-vuetify", text: "Vuetify", color: "blue" },
          ],
        },
        {
          id: "semicolon0103",
          src: require("../assets/semicolon0103/aoha_icon.webp"),
          to: "https://semicolon0103.com/",
          title: "Aioi Aoha's Workshop",
          tag: [
            { icon: "mdi-vuejs", text: "Vue 3", color: "#57bc85" },
            { icon: "mdi-vuetify", text: "Vuetify", color: "blue" },
          ],
        },
        {
          id: "im3py",
          src: require("../assets/im3py/im3py_ico.webp"),
          to: "https://sui828.github.io/",
          title: "生成物置き場",
          tag: [
            { icon: "mdi-vuejs", text: "Vue 3", color: "#57bc85" },
            { icon: "mdi-vuetify", text: "Vuetify", color: "blue" },
          ],
        },
        {
          id: "portfolio",
          src: require("../assets/icon.webp"),
          to: "https://sui828.github.io/",
          title: "ポートフォリオ",
          tag: [
            { icon: "mdi-vuejs", text: "Vue 3", color: "#57bc85" },
            { icon: "mdi-vuetify", text: "Vuetify", color: "blue" },
          ],
        },
      ],
    };
  },
  methods: {
    QueryIs: function(){
      if(this.$route.query.p === undefined){
        this.page = "/"
      }else{
        this.page = "/" + this.$route.query.p
      }
      console.log(this.page);
      if(this.page !== "/"){
        this.$router.push(this.page)
      }
    },
  },
  mounted(){
    this.QueryIs();
  },
};
</script>
