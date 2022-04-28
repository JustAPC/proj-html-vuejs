<template>
  <div class="d-flex jcbetween">
    <div class="logo-container pt-4 ps-6">
      <img src="../../assets/images/logotype.png" alt="logo phlox" class="jcs w-35" />
    </div>

    <div class="header-menu">
      <ul class="d-flex aicenter">
        <li
          v-for="(elm, i) in menuListItems"
          :key="i"
          class="align-items-center text-uppercase pt-4 mx-3"
          :class="{ active: elm.activePage }"
        >
          <a :href="elm.link" class="">{{ elm.title }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {},

  data() {
    return {
      menuListItems: [
        {
          title: "Home",
          link: "#",
          activePage: true,
        },
        {
          title: "About",
          link: "#",
          activePage: false,
        },
        {
          title: "Projects",
          link: "#",
          activePage: false,
        },
        {
          title: "Services",
          link: "#",
          activePage: false,
        },
        {
          title: "Blog",
          link: "#",
          activePage: false,
        },
        {
          title: "Contact",
          link: "#",
          activePage: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/styles/mystyles.scss";
@import "../../assets/styles/mystyle.css";

.active {
  border-top: 3px solid $border-color-white1;
  a {
    color: $text-color-white1;
  }
}

ul li {
  list-style-type: none;
}

li a {
  color: $text-color-white2;
  text-decoration: none;
}
</style>
