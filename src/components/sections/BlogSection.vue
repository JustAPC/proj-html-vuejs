<template>
  <div class="pt-5">
    <div class="pt-5">
      <div class="col-10 mx-auto">
        <div class="green-rule border"></div>
        <span class="text-white fs-5">BLOG</span>
        <div class="d-flex justify-content-between align-items-center pt-3">
          <span class="text-uppercase text-white fs-1 fw-bold"
            >the recent news you must read it</span
          >
          <button class="view-button text-uppercase">View All</button>
        </div>
        <div class="d-flex news-container">
          <NewsCard
            v-for="(elm, i) in newsList"
            :key="i"
            :bgImg="elm.bgImg"
            :date="elm.date"
            :author="elm.author"
            :title="elm.title"
            :body="elm.body"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NewsCard from "../partials/NewsCard.vue";

export default {
  name: "BlogSection",

  components: {
    NewsCard,
  },

  data() {
    return {
      newsList: [
        {
          bgImg: require("../../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg"),
          date: "july 4, 2019",
          author: "paul",
          title: "Canadian Consulting Firm acquired by UK Giant",
          body: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
        {
          bgImg: require("../../assets/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg"),
          date: "july 4, 2019",
          author: "paul",
          title: "Canadian Consulting Firm acquired by UK Giant",
          body: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";

.view-button {
  letter-spacing: 3px;
  border: 0;
  padding: 20px 45px;
  background-color: $bg-color-green;
  &:hover {
    background-color: $bg-color-red;
    color: $text-color-white1;
  }
}

.news-container {
  padding-bottom: 300px;
}
</style>
