<script lang="ts" setup>

</script>

<template>
   <NuxtLink to="/news/2" class="h-48 relative overflow-hidden rounded-lg">
      <div class="bg1">
         <div class="bg-linear"></div>
         <img class="h-full home-news longer-width" src="@/assets/img/news1.jpg">
      </div>
      <h5 class="text-white font-poppins-600 absolute bottom-10 left-10 z-10">O‘quv soati bo‘lib o‘tdi</h5>
   </NuxtLink>
</template>
<style lang="scss" scoped>
.bg1 {
   display: flex;
   align-items: center;
   justify-content: center;
   width: 100%;
   height: 100%;

   &:hover {
      scale: 1.05;
   }
}

.bg-linear {
   background-image: linear-gradient(transparent, #000);
   position: absolute;
   background-image: linear-gradient(transparent, #000);
   z-index: 1;
   width: 100%;
   height: 100%;
   opacity: 0.4;
}

img.longer-width {
   min-width: auto !important;
   max-width: auto !important;
   height: 100% !important;
}

.news-section .news-grid .news-item .bg img.home-news {
   min-width: 100%;
   min-height: 100%;
   transition: 0.3s ease-in all;
}
</style>