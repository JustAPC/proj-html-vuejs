<template>
  <div>
    <div class="get-started-hero">
      <div class="text-center get-started-text-container text-white">
        <div>
          <h1 class="text-uppercase fw-bold">Let's talk about work</h1>
          <p>A wonderful serenity has taken possession Far far away, behind the word mountains.</p>
          <button class="get-started-button text-uppercase">get started</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GetStarted",
  props: {},
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.get-started-hero {
  height: 482px;
  width: 100%;
  background-image: url(../../assets/images/business-people-working-together-on-project-and-B3MZ4TX.jpg);
}

.get-started-text-container {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.get-started-button {
  border: 0;
  letter-spacing: 3px;
  padding: 20px 50px;
  color: $text-color-white1;
  background-color: $bg-color-violet;
  &:hover {
    background-color: $bg-color-blue;
  }
}
</style>
