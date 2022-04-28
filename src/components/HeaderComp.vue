<template>
  <div>
    <header class="p-relative d-flex">
      <div class="h-100 flex-grow waves-bg"></div>
      <div class="h-100 w-67 hero-img"></div>

      <div class="container-p p-absolute">
        <NavbarItems />

        <div class="w-90 hero-text-container jcbetween">
          <div>
            <div class="d-inline-block divider"></div>
            <span class="text-white text-uppercase">Always the best way you need it</span>
          </div>
          <div class="w-40">
            <h1 class="text-white text-uppercase hero-text">the best business consulting</h1>
          </div>
          <div>
            <button class="text-uppercase">Read More</button>
            <div class="d-inline-block"><i class="fa-solid fa-play play-icon"></i></div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
import NavbarItems from "./partials/NavbarItems.vue";

export default {
  name: "HeaderComp",
  components: {
    NavbarItems,
  },
  props: {},
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";
@import "../assets/styles/mystyle.css";

header {
  height: 100vh;
  width: 100vw;
}

.container-p {
  top: 0;
  left: 45px;
  width: 90%;
  margin: 0 auto;
}

.waves-bg {
  background-image: url(../assets/images/violet-bg-1.png);
}

.hero-img {
  background-image: url(../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg);
  background-size: cover;
}

.hero-text-container {
  padding-top: 250px;
  height: 720px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;

  span {
    letter-spacing: 3px;
    font-size: 1.1rem;
  }

  h1 {
    font-weight: 1000;
  }
}

.hero-text {
  font-size: 6rem;
  line-height: 90px;
}

.divider {
  width: 50px;
  height: 3px;
  background-color: $bg-color-green;
  margin-right: 20px;
}

button {
  padding: 20px 60px;
  border: 0;
  letter-spacing: 3px;
  background-color: $bg-color-green;
  &:hover {
    color: white;
    background-color: $bg-color-red;
  }
}

.play-icon {
  margin-left: 30px;
  color: $text-color-green;
  padding: 18px;
  border-radius: 50%;
  border: 2px solid $text-color-white1;
  cursor: pointer;
}
</style>
