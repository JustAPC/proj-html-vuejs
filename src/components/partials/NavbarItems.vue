<template>
  <div class="d-flex jcbetween">
    <div class="logo-container pt-4 ps-6">
      <img src="../../assets/images/logotype.png" alt="logo phlox" class="jcs w-35" />
    </div>

    <div class="header-menu">
      <ul class="d-flex aicenter">
        <li v-for="(elm, i) in menuListItems" :key="i" class="text-uppercase pt-4 active">
          <a :href="elm.link" class="px-3">{{ elm.title }}</a>
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
          active: true,
        },
        {
          title: "About",
          link: "#",
          active: false,
        },
        {
          title: "Projects",
          link: "#",
          active: false,
        },
        {
          title: "Services",
          link: "#",
          active: false,
        },
        {
          title: "Blog",
          link: "#",
          active: false,
        },
        {
          title: "Contact",
          link: "#",
          active: false,
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
  border-top: 2px solid $border-color-white1;
  color: $text-color-white1;
}

ul li {
  list-style-type: none;
}

li a {
  color: $text-color-white2;
  text-decoration: none;
}
</style>
