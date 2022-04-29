<template>
  <div class="violet-bg" style="height: 1000px">
    <div class="mx-auto col-10 pt-6 pb-5">
      <div class="text-white">
        <div class="text-center text-uppercase fs-5">Testimonial</div>
        <div class="green-rule float-end me-0"></div>
      </div>
      <div class="text-white text-end offset-7 col-5 pt-3 text-uppercase fs-1 fw-bold">
        What's the customer say about our work
      </div>
    </div>

    <div class="witnesses-banner col-11 offset-1">
      <WitnessesBar />
    </div>
  </div>
</template>

<script>
import WitnessesBar from "../partials/WitnessesBar.vue";

export default {
  name: "TestimonialSection",
  props: {},
  components: {
    WitnessesBar,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.witnesses-banner {
  height: 350px;
  background-color: $bg-color-white;
  z-index: 1000;
}
</style>
