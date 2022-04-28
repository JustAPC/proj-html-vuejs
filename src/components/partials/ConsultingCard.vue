<template>
  <div class="d-flex flex-wrap card-box justify-content-between p-5">
    <div v-for="(elm, i) in consultingList" :key="i" class="col-5 d-flex card-container pt-2">
      <div class="pe-5">
        <img :src="elm.logo" :alt="`logo di ${elm.type}`" />
      </div>
      <div>
        <h4 class="text-uppercase fw-bold">{{ elm.type }} Consulting</h4>
        <p>{{ elm.text }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ConsultingCard",
  props: {},

  data() {
    return {
      consultingList: [
        {
          type: "Statistical",
          logo: require("../../assets/images/graph-icon.png"),
          text: "When, while lovely valley teems with vapour around me and eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
        {
          type: "Digital",
          logo: require("../../assets/images/megaphone-icon.png"),
          text: "When, while lovely valley teems with vapour around me and eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
        {
          type: "Banking",
          logo: require("../../assets/images/wallet-icon.png"),
          text: "When, while lovely valley teems with vapour around me and eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
        {
          type: "Enterprise",
          logo: require("../../assets/images/bullseye-icon.png"),
          text: "When, while lovely valley teems with vapour around me and eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.card-box {
  padding-top: 8rem;
}

.card-container {
  padding-bottom: 130px;
}

p {
  color: $text-color-violet2;
  font-size: 1.1em;
}
</style>
