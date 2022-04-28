<template>
  <ConsultantSection />
</template>

<script>
import ConsultantSection from "./ConsultantSection.vue";

export default {
  name: "MainComp",

  components: {
    ConsultantSection,
  },

  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";

.pt-6 {
  padding-top: 5rem;
}

.consultant-section {
  height: 95vh;
}

h3 {
  color: $text-color-violet1;
}

.divider {
  height: 3px;
  width: 60%;
  background-color: $bg-color-green;
  margin-left: 500px;
}
</style>
