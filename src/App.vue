<template>
  <div id="app">
    <HeaderComp />
  </div>
</template>

<script>
import "./assets/styles/mystyles.scss";

import HeaderComp from "./components/HeaderComp.vue";

export default {
  name: "App",
  components: {
    HeaderComp,
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
</style>
