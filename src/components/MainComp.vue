<template>
  <div>
    <ConsultantSection />
    <AboutUsSection />
    <ProjectSection />
    <TestimonialSection />
    <BlogSection />
    <GetStarted />
  </div>
</template>

<script>
import ConsultantSection from "./sections/ConsultantSection.vue";
import AboutUsSection from "./sections/AboutUsSection.vue";
import ProjectSection from "./sections/ProjectSection.vue";
import TestimonialSection from "./sections/TestimonialSection.vue";
import BlogSection from "./sections/BlogSection.vue";
import GetStarted from "./sections/GetStarted.vue";

export default {
  name: "MainComp",

  components: {
    ConsultantSection,
    AboutUsSection,
    ProjectSection,
    TestimonialSection,
    BlogSection,
    GetStarted,
  },

  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";
</style>
