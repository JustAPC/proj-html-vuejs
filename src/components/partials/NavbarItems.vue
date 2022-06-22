<template>
   <div class="navbar-container w-100 position-absolute">
      <div class="d-flex justify-content-between align-items-center mx-5 py-4" height="50px">
         <div>
            <img src="../../assets/images/logotype.png" alt="" class="logo" />
         </div>

         <div>
            <ul class="d-flex align-items-center p-0 m-0">
               <li v-for="(elm, i) in menuListItems" :key="i">
                  <a :href="elm.url" class="text-uppercase py-4 mx-3" :class="{ active: elm.activePage }">
                     {{ elm.page }}
                  </a>
               </li>
            </ul>
         </div>
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
                  page: "Home",
                  url: "#",
                  activePage: true,
               },
               {
                  page: "About",
                  url: "#",
                  activePage: false,
               },
               {
                  page: "Projects",
                  url: "#",
                  activePage: false,
               },
               {
                  page: "Services",
                  url: "#",
                  activePage: false,
               },
               {
                  page: "Blog",
                  url: "#",
                  activePage: false,
               },
               {
                  page: "Contact",
                  url: "#",
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

   .navbar-container {
      z-index: 2;
      top: 0;
      left: 0;
   }

   .logo {
      width: 36%;
   }

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

   a:hover {
      color: $text-color-white1;
   }
</style>
