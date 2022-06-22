<template>
   <div class="waves-bg col-4">
      <div class="hero-description d-flex flex-column justify-content-between position-absolute">
         <div>
            <div class="green-rule"></div>
            <span class="text-white text-uppercase fs-5">Always the best way you need it</span>
         </div>

         <div class="w-40">
            <h1 class="hero-title text-white text-uppercase">the best business consulting</h1>
         </div>

         <div>
            <button class="text-uppercase">Read More</button>
            <div class="d-inline-block"><i class="fa-solid fa-play play-icon"></i></div>
         </div>
      </div>
   </div>
</template>

<script>
   export default {
      name: "HeroDescription",
   };
</script>

<style scoped lang="scss">
   @import "../../assets/styles/mystyles.scss";

   .waves-bg {
      background-image: url(../../assets/images/violet-bg-1.png);
   }

   .hero-description {
      padding-top: 300px;
      padding-left: 150px;
      height: 750px;
      z-index: 1000;
   }

   .hero-title {
      font-size: 6rem;
      line-height: 90px;
      font-weight: bold;
   }

   button {
      padding: 20px 60px;
      border: 0;
      letter-spacing: 3px;
      background-color: $bg-color-green;
      &:hover {
         color: white;
         background-color: $bg-color-red;
      }
   }

   .play-icon {
      margin-left: 30px;
      color: $text-color-green;
      padding: 18px 20px;
      border-radius: 50%;
      border: 2px solid $text-color-white1;
      cursor: pointer;
      &:hover {
         background-color: $text-color-red;
         color: white;
         border: 2px solid white;
      }
   }
</style>
