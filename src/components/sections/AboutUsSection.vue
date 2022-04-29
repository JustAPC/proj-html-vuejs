<template>
  <div class="violet-bg">
    <div class="d-flex">
      <div class="hero-img col-7 d-flex align-items-end position-relative">
        <div class="get-started-banner position-absolute d-flex align-items-center">
          <div class="offset-2 col-3">
            <h2 class="banner-title ps-5">We help to deliver the business case</h2>
          </div>

          <div class="col-4 offset-1 get-started-description">
            When, while lovely valley teems with vapour around meand meridian sun strikes the upper
            impenetrable foliage of my trees, and but a thousand unknown
          </div>

          <div class="get-started d-flex flex-grow-1 h-100 align-items-end justify-content-end">
            <button class="get-started-button">get started</button>
          </div>
        </div>
      </div>

      <div class="about-us-text-bg col-5 pt-5">
        <AboutUsText />
      </div>
    </div>
  </div>
</template>

<script>
import AboutUsText from "../partials/AboutUsText.vue";
export default {
  name: "AboutUsSection",
  components: {
    AboutUsText,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.hero-img {
  height: 900px;
  background-image: url(../../assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg);
  background-repeat: no-repeat;
}

.about-us-text-bg {
  height: 1340px;
  background-image: url(../../assets/images/violet-bg-2.png);
  background-repeat: no-repeat;
}

.get-started-banner {
  bottom: -300px;
  left: 0;
  height: 330px;
  width: 1750px;
  background-color: $bg-color-green;
  z-index: 1000;
}

.banner-title {
  text-transform: uppercase;
  font-weight: bold;
  color: $text-color-violet1;
}

.get-started-description {
  padding-left: 5rem;
  padding-right: 3rem;
  color: $text-color-violet2;
}

.get-started-button {
  text-transform: uppercase;
  padding: 20px 50px;
  border: 0;
  color: $text-color-white1;
  background-color: $bg-color-red;
  letter-spacing: 2px;
  &:hover {
    background-color: $bg-color-violet;
  }
}
</style>
