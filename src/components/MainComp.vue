<template>
  <div>
    <ConsultantSection />
    <AboutUsSection />
    <ProjectSection />
  </div>
</template>

<script>
import ConsultantSection from "./sections/ConsultantSection.vue";
import AboutUsSection from "./sections/AboutUsSection.vue";
import ProjectSection from "./sections/ProjectSection.vue";

export default {
  name: "MainComp",

  components: {
    ConsultantSection,
    AboutUsSection,
    ProjectSection,
  },

  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";
</style>
