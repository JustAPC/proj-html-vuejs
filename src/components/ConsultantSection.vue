<template>
  <div class="consultant-section container pt-5">
    <div class="p-5 d-flex align-items-center">
      <div>
        <h3 class="text-uppercase fw-bold">our consultants can help you</h3>
      </div>
      <div class="d-inline-block divider position-absolute"></div>
    </div>
    <ConsultingCard />
  </div>
</template>

<script>
import ConsultingCard from "./partials/ConsultingCard.vue";
export default {
  name: "ConsultantSection",
  props: {},

  components: {
    ConsultingCard,
  },
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
