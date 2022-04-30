<template>
  <div>
    <div class="text-white pt-5 position-relative">
      <img :src="bgImg" alt="" class="col-12 px-3" />
      <div class="position-absolute news-container">
        <div class="pt-5 ps-5 col-9 h-100">
          <div class="ps-5">
            <span>{{ date }}</span>
            <span class="ps-5">by {{ author }}</span>
            <h3 class="py-3">{{ title }}</h3>
            <p>{{ body }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VueCard",
  props: {
    bgImg: String,
    date: String,
    author: String,
    title: String,
    body: String,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.news-container {
  bottom: -75px;
  right: 16px;
  z-index: 1000;
  background-color: white;
  width: 600px;
  height: 300px;
}

span {
  color: $text-color-red;
}

h3 {
  color: $text-color-black;
}

p {
  color: $text-color-grey;
}
</style>
