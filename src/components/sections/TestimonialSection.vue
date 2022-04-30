<template>
  <div class="violet-bg pb-5">
    <div class="mx-auto col-10 pt-6 pb-5">
      <div class="text-white">
        <div class="text-center text-uppercase fs-5">Testimonial</div>
        <div class="green-rule float-end me-0"></div>
      </div>
      <div class="text-white text-end offset-7 col-5 pt-3 text-uppercase fs-1 fw-bold">
        What's the customer say about our work
      </div>
    </div>

    <div>
      <div class="squares-bg border"></div>
      <div class="witnesses-banner col-11 offset-1">
        <WitnessesBar />
      </div>
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
  z-index: 2;
}

.squares-bg {
  position: absolute;
  height: 1000px;
  left: -2px;
  bottom: 0;
  background-repeat: no-repeat;
  background-image: url(../../assets/images/violet-bg-3.png);
  z-index: 1;
}
</style>
