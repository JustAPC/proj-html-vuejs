<template>
  <div>
    <ConsultantSection />
    <AboutUsSection />
  </div>
</template>

<script>
import ConsultantSection from "./ConsultantSection.vue";
import AboutUsSection from "./AboutUsSection.vue";

export default {
  name: "MainComp",

  components: {
    ConsultantSection,
    AboutUsSection,
  },

  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";
</style>
