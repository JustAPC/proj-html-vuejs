<template>
  <div id="app">
    <HeaderComp />
    <MainComp />
    <FooterComp />
  </div>
</template>

<script>
import "./assets/styles/mystyles.scss";

import HeaderComp from "./components/HeaderComp.vue";
import MainComp from "./components/MainComp.vue";
import FooterComp from "./components/FooterComp.vue";

export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
  },
};
</script>

<style lang="scss">
@import "bootstrap";
@import "./assets/styles/mystyles.scss";
@import "./assets/styles/mystyle.css";
@import url("https://fonts.googleapis.com/css2?family=Radio+Canada&display=swap");
#app {
  font-family: "Radio Canada", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.green-rule {
  width: 50px;
  height: 3px;
  background-color: $bg-color-green;
  margin-right: 20px;
  display: inline-block;
}

.pt-6 {
  padding-top: 7rem;
}

body {
  background-color: $bg-color-violet;
}
</style>
