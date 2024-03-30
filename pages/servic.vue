<script lang="ts" setup>

</script>

<template>
   <div class="container">
      <h2 class="text-center my-16">Bizning xizmatlarimiz</h2>
      <div class="grid grid-cols-3 gap-6">
         <div class="flex flex-col card-box rounded-xl">
            <div class="card-img h-60 flex justify-center items-center rounded-lg">
                <img class="max-w-52" src="@/assets/img/uzImei.png" alt="">
            </div>
            <div class="p-4 px-6 min-h-36">
               <h4>UzIMEI</h4>
               <p class="text-sm mt-2">Mobil qurilmangizni IMEI - kodini ro'yxatdan o'tkazing</p>
            </div>
            <a href="https://uzimei.uz/" class="p-4 px-6">Ko'proq</a>
         </div>
         <div class="flex flex-col card-box rounded-xl">
            <div class="card-img h-60 flex justify-center items-center rounded-lg">
                <img class="max-w-52" src="@/assets/img/mnp.svg" alt="">
            </div>
            <div class="p-4 px-6 min-h-32">
               <h4>Mobil aloqa tarmoqlarining abonent raqamini ko'chirish xizmati</h4>
               <p class="text-sm mt-2">MNP</p>
            </div>
            <a href="https://mnp.uz/" class="p-4 px-6">Ko'proq</a>
         </div>
         <div class="flex flex-col card-box rounded-xl">
            <div class="card-img h-60 flex justify-center items-center rounded-lg">
                <img class="max-w-52" src="@/assets/img/uzEx.png" alt="">
            </div>
            <div class="p-4 px-6 min-h-32">
               <h4>Qisqa raqamlar</h4>
               <p class="text-sm mt-2">Qisqa raqamlar onlayn auksioni</p>
            </div>
            <a href="https://mobilraqam.uzex.uz/" class="p-4 px-6">Ko'proq</a>
         </div>
      </div>
   </div>

</template>
<style lang="scss" scoped>
.our-services-section .service-card {
    background: #FFFFFF;
    box-shadow: 0px 0px 20px rgba(24, 47, 67, 0.2);
    border-radius: 6px;
}
.card-img{
   background-image: linear-gradient(216deg, #1D9BD8 -13%, #312C7F 96%);
}
.card-box {
   box-shadow: 0px 0px 20px rgba(24, 47, 67, 0.2);
}

</style>