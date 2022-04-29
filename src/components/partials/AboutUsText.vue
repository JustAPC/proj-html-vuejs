<template>
  <div>
    <div class="about-us-text-container d-flex flex-column justify-content-between">
      <div class="d-flex">
        <div class="divider me-3"></div>
        <span class="text-uppercase text-white"> About Us</span>
      </div>

      <div class="col-8 ms-4">
        <h2 class="text-uppercase text-white strategy-text">We make your strategy work</h2>
      </div>

      <div class="about-us-description col-8 ms-2">
        When, while lovely valley teems with vapour around meand eridian sun strikes the upper
        impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear
        the buzz of the little world among the stalks, and grow familiar indescribable form of the
        insects and flies, then I feel the presence of the Almighty.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutUsText",
  props: {},
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";
.divider {
  margin-top: 0.9rem;
  width: 50px;
  height: 3px;
  background-color: $bg-color-green;
}

.about-us-text-container {
  padding-left: 70px;
  padding-top: 200px;
  height: 550px;
}

.strategy-text {
  font-weight: bold;
  font-size: 3.5rem;
}

.about-us-description {
  color: $text-color-white4;
}
</style>
