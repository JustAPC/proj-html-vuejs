<template>
  <div class="d-flex justify-content-between">
    <div v-for="(elm, i) in clientCard" :key="i">
      <div
        class="clients-bg"
        :style="{ backgroundImage: 'url(' + elm.img + ')' }"
        @mouseover="mouseOver(i)"
        @mouseleave="hover = false"
      >
        <div
          class="h-100 d-flex align-items-end hover-container"
          v-show="hover && i === mouseOverIndex"
        >
          <div class="d-flex justify-content-between px-3 pb-3 w-100">
            <div>
              <h5 class="fw-bold">{{ elm.name }}</h5>
              <span>{{ elm.category }}</span>
            </div>
            <div>
              <button class="client-button"><i class="fa-solid fa-plus"></i></button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ClientCards",

  data() {
    return {
      clientCard: [
        {
          name: "Dry",
          category: "uncategorized",
          img: require("../../assets/images/DRY-1-790x592.jpg"),
        },
        {
          name: "Notvine",
          category: "uncategorized",
          img: require("../../assets/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg"),
        },
        {
          name: "Vizeon",
          category: "uncategorized",
          img: require("../../assets/images/z1el4c4p-790x592.jpg"),
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

.clients-bg {
  width: 516px;
  height: 385px;
  background-size: cover;
}

.hover-container {
  background-color: rgba($color: red, $alpha: 0.5);
}

span {
  color: $text-color-white4;
}

h5,
span {
  text-shadow: 2px 2px 10px black;
}

.client-button {
  color: white;
  padding: 20px 22px;
  background-color: $bg-color-violet;
  border: 0;
  &:hover {
    background-color: $bg-color-grey;
  }
}
</style>
