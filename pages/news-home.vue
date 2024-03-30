<script lang="ts" setup>
import Card from './news/Card.vue'
</script>

<template>
   <div class="container">
      <div class="flex justify-between items-end my-10">
         <h2>Yangiliklar</h2>
         <NuxtLink to="/news">Hammasini ko'rish</NuxtLink>
      </div>
      <div class="grid grid-cols-4 gap-5">
         <NuxtLink to="/news/2" class="col-span-3 relative overflow-hidden h-[820px] rounded-lg">
            <div class="bg">
               <div class="bg-linear"></div>
               <img class="home-news longer-width" src="@/assets/img/news1.jpg">
            </div>
            <h1 class="text-white absolute bottom-10 left-10 z-10">O‘quv soati bo‘lib o‘tdi</h1>
         </NuxtLink>
         <div class="col-span-1 flex flex-col gap-4">
            <Card />
            <Card />
            <Card />
            <Card />
         </div>
      </div>

   </div>
</template>
<style lang="scss" scoped>
.bg {
   position: absolute;
   display: flex;
   align-items: center;
   justify-content: center;
   // width: 100%;
   height: 100%;
   &:hover{
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