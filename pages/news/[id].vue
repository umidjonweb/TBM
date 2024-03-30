<script lang="ts" setup>

</script>

<template>
   <NuxtLayout>
      <div class="container !my-20">
         <div class="grid grid-cols-3 gap-12 pr-20">
            <div class="col-span-2">
               <h3 class="my-7">O‘quv soati bo‘lib o‘tdi</h3>

               <img class="w-full" src="@/assets/img/news1.jpg" alt="">
               <div class="flex flex-col gap-4 mt-3">
                  <p class="text-sm">mar 28 2024</p>
                  <p>Zoom platformasi orqali onlayn tarzda o‘tkazilgan mazkur o‘quv soatida Mobil qurilmalarni ro‘yxatga
                     olish
                     xizmati yetakchi mutaxassisi B.Qurbonboyev "Mobil qurilmalarni ro‘yxatga olish soxasida boshqa
                     mutasaddi
                     vazirlik va idoralar bilan o‘zaro hamkorlikka qaratilgan chora-tadbirlar" mavzusida xodimlarga
                     umumiy
                     tushunchalar berib o‘tdi.</p>
                  <p>Qizg‘in bahs-munozaralarga boy tarzida o‘tgan mazkur o‘quv soati yakunida xodimlar o‘zlari
                     qiziqtirgan savollarga javob olishdi.</p>
               </div>
            </div>
            <div class="border border-black/10 rounded-xl px-5 col-span-1">
               <div v-for="item in 8" :key="item" class="flex gap-6 py-5 border-b border-b-black/10">
                  <img class="w-16 h-16 rounded" src="@/assets/img/news1.jpg" alt="">
                  <div class="flex flex-col justify-between">
                     <NuxtLink to="/news/4" class="font-poppins-600">O‘quv soati bo‘lib o‘tdi</NuxtLink>
                     <p class="text-xs pb-1">mar 28 2024</p>
                  </div>
               </div>
            </div>
         </div>
      </div>
   </NuxtLayout>
</template>
<style scoped>

</style>