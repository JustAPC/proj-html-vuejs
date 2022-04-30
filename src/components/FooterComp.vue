<template>
  <div class="pt-5">
    <div class="d-inline-block col-10 offset-1 py-5">
      <div class="d-flex justify-content-between pb-5">
        <div>
          <img src="../assets/images/logotype-2-139x23.png" alt="" />
        </div>

        <div>
          <ul class="d-flex align-items-center h-100">
            <li v-for="(elm, i) in menuListItems" :key="i">
              <a :href="elm.link" class="mx-2">{{ elm.title }}</a>
            </li>
          </ul>
        </div>

        <div class="social-icons">
          <a href="#"><i class="fa-brands fa-instagram"></i></a>
          <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
          <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
          <a href="#"><i class="fa-brands fa-twitter"></i></a>
        </div>
      </div>

      <hr />

      <div class="pt-3">
        <div class="d-flex justify-content-between info-section">
          <div>
            <a href="#">Terms of use</a>
            <div><a href="#">Privacy Environmental Policy</a></div>
          </div>

          <div>Copyright &#169; 2020 Phlox Consulting.All Rights Reserved.</div>
        </div>
      </div>
    </div>

    <div class="col-1 d-inline-block text-white ps-3">
      <a href=""><i class="fa-solid fa-arrow-up-long arrow-up"></i></a>
      <a href="" class="ps-3"><i class="fa-solid fa-comment comment-icon"></i></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComp",
  props: {},
  data() {
    return {
      menuListItems: [
        {
          title: "Home",
          link: "#",
        },
        {
          title: "About",
          link: "#",
        },
        {
          title: "Projects",
          link: "#",
        },
        {
          title: "Services",
          link: "#",
        },
        {
          title: "Blog",
          link: "#",
        },
        {
          title: "Contact",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/styles/mystyles.scss";

ul li {
  list-style-type: none;
}

li a {
  color: $text-color-white4;
  text-decoration: none;
  text-transform: uppercase;
  &:hover {
    color: white;
  }
}

.social-icons {
  display: flex;
  align-items: center;
  & a {
    text-decoration: none;
    color: white;
    margin-left: 20px;
  }
}

hr {
  color: grey;
}

.info-section {
  color: $text-color-white4;
  & a {
    text-decoration: none;
    color: $text-color-white4;
  }
}

.arrow-up {
  color: black;
  font-size: 0.7em;
  padding: 11px 13px;
  border-radius: 50%;
  background-color: white;
}

.comment-icon {
  font-size: 1.4em;
  color: white;
  background-color: $bg-color-blue;
  padding: 18px;
  border-radius: 50%;
  transform: rotateY(180deg);
}
</style>
