<template>
  <div class="d-flex">
    <div
      class="col-4 card-container position-relative"
      v-for="(elm, i) in witnessesList"
      @mouseover="mouseOver(i)"
      @mouseleave="hover = false"
      :style="[
        hover && i === mouseOverIndex
          ? { backgroundImage: 'url(' + elm.img + ')' }
          : { backgroundImage: 'none' },
      ]"
      :key="i"
    >
      <div class="pt-5 mx-5 position-absolute">
        <p class="col-10" :class="{ witnessText: hover && i === mouseOverIndex }">
          {{ elm.speech }}
        </p>
        <h4 class="pt-4 fw-bold" :class="{ witnessName: hover && i === mouseOverIndex }">
          {{ elm.name }}
        </h4>
        <span :class="{ witnessText: hover && i === mouseOverIndex }">{{ elm.company }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WitnessesBar",
  props: {},
  data() {
    return {
      witnessesList: [
        {
          name: "Vera Duncan",
          company: "Amazon Inc.",
          img: require("../../assets/images/oliver-ragfelt-488196-2.jpg"),
          speech:
            "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little",
        },
        {
          name: "Oliver Ragfeld",
          company: "Boolean Careers",
          img: require("../../assets/images/oliver-ragfelt-488196-unsplash.jpg"),
          speech:
            "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little",
        },
        {
          name: "John Doe",
          company: "Web Development",
          img: require("../../assets/images/oliver-ragfelt-488196-unsplash.jpg"),
          speech:
            "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little",
        },
      ],

      hover: false,
      mouseOverIndex: null,
    };
  },

  methods: {
    mouseOver(index) {
      this.hover = true;
      this.mouseOverIndex = index;
    },
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

p,
span {
  color: $text-color-violet3;
}

.no-bg-card {
  background-image: none;
}

.card-container {
  cursor: pointer;
  height: 350px;
  background-size: cover;
  background-position: center;
}

.witnessName {
  color: $text-color-white1;
}

.witnessText {
  color: $text-color-white2;
}
</style>
