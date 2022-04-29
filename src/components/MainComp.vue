<template>
  <div>
    <ConsultantSection />
    <AboutUsSection />
    <ProjectSection />
    <TestimonialSection />
  </div>
</template>

<script>
import ConsultantSection from "./sections/ConsultantSection.vue";
import AboutUsSection from "./sections/AboutUsSection.vue";
import ProjectSection from "./sections/ProjectSection.vue";
import TestimonialSection from "./sections/TestimonialSection.vue";

export default {
  name: "MainComp",

  components: {
    ConsultantSection,
    AboutUsSection,
    ProjectSection,
    TestimonialSection,
  },

  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";
</style>
