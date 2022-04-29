<template>
  <div class="violet-bg text-white">
    <div class="col-10 mx-auto">
      <div>
        <div class="green-rule"></div>
        <span class="text-uppercase fs-5">Project</span>
      </div>

      <div class="d-flex justify-content-between">
        <h1 class="col-6 text-uppercase fw-bold pt-4">
          Our expert trusted consultants help clients
        </h1>

        <div class="d-flex align-items-center">
          <i class="fa-solid fa-arrow-left-long arrows me-3"></i>
          <i class="fa-solid fa-arrow-right-long arrows"></i>
        </div>
      </div>

      <ClientCards class="py-5" />
    </div>
  </div>
</template>

<script>
import ClientCards from "../partials/ClientCards.vue";
export default {
  name: "ProjectSection",
  components: {
    ClientCards,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.arrows {
  cursor: pointer;
  font-size: 0.9em;
  background-color: #36354c;
  color: $text-color-green;
  padding: 20px;
}
</style>
