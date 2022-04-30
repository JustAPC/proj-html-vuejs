<template>
  <div>
    <ConsultantSection />
    <AboutUsSection />
    <ProjectSection />
    <div class="position-relative">
      <TestimonialSection />
      <div class="squares-bg"></div>
    </div>
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

.squares-bg {
  position: absolute;
  height: 1712px;
  width: 960px;
  top: 304px;
  z-index: -1;
  background-size: cover;
  background-repeat: no-repeat;
  background-image: url(../assets/images/violet-bg-3.png);
}
</style>
