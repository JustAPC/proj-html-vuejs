<template>
  <div class="consultant-section pt-5">
    <div class="pt-5 d-flex align-items-center offset-2">
      <div class="pt-5 col-4 me-4">
        <h3 class="text-uppercase fw-bold">our consultants can help you</h3>
      </div>
      <div class="divider col-6 flex-grow-1"></div>
    </div>

    <div class="container">
      <ConsultingCard />
    </div>
  </div>
</template>

<script>
import ConsultingCard from "../partials/ConsultingCard.vue";

export default {
  name: "ConsultantSection",
  props: {},

  components: {
    ConsultingCard,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.consultant-section {
  height: 95vh;
}

h3 {
  color: $text-color-violet1;
}

.divider {
  height: 3px;
  background-color: $bg-color-green;
}
</style>
