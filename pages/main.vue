<script lang="ts" setup>

</script>

<template>
   <div class="banner-content" >
      <div class="container">
         <h3 class="mb-24 uppercase text-white font-poppins-700 text-[38px] w-[52%]">
            «O'ZBEKISTON TELEKOMMUNIKATSIYA TARMOQLARINI BOSHQARISH RESPUBLIKA MARKAZI» DAVLAT UNITAR KORXONASI
         </h3>
         <button class="group py-4 px-8 rounded-lg hover:bg-[#2ad655] bg-[#d6e138] font-poppins-500">
            <nuxt-link to="main-center" class="group-hover:text-white" href="https://rtmc.uz/about-center">
               Qo'shimcha ma'lumot <span class="ri-xl ri-arrow-right-s-line"></span>
            </nuxt-link>
         </button>
      </div>
   </div>
</template>
<style lang="scss">
  .banner-content {
   background-image: url('../assets/img/main.jpg');
    padding: 80px 0 100px;
    top: 0;
    width: 100%;
    min-height: 580px;
    display: flex;
    align-items: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
}
</style>