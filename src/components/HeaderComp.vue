<template>
   <div>
      <header class="d-flex justify-content-center position-relative text-center">
         <NavbarItems />
      </header>

      <main class="hero-section d-flex">
         <HeroDescription />
         <div class="hero-img col-8"></div>
      </main>
   </div>
</template>

<script>
   import NavbarItems from "./partials/NavbarItems.vue";
   import HeroDescription from "./partials/HeroDescription.vue";

   export default {
      name: "HeaderComp",
      components: {
         NavbarItems,
         HeroDescription,
      },
      props: {},
   };
</script>

<style scoped lang="scss">
   @import "../assets/styles/mystyles.scss";
   @import "../assets/styles/mystyle.css";

   .hero-section {
      height: 100vh;
   }

   .hero-img {
      background-image: url(../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg);
      background-size: cover;
      z-index: 0;
   }
</style>
