<script lang="ts" setup>

const _items = ref([
   {
      questinary: "Mobil aloqa operatori o‘zgartirilganda, ko‘rsatilayotgan xizmat sifati qoniqtirmasa, dastlabki operatorga qayta o‘tish mumkinmi?",
      answer: "Siz 30 taqvim kuni o‘tganidan so‘ng bu xizmatdan foydalanishingiz mumkin.",
      visible: false
   },
   {
      questinary: "Agar mobil aloqa operatori o‘zgartirilsa, raqamingiz shakli saqlanadimi?",
      answer: "Ko‘chirilgan raqamlar o‘z shaklini va to‘kisligini saqlab qoladi",
      visible: false
   },
   {
      questinary: "Qaysi operatorlar GSM standarti bo‘yicha faoliyat olib boradi?",
      answer: "Hozirgi kunda O‘zbekiston Respublikasi hududida 5 ta mobil aloqa operatori GSM aloqa standarti bo‘yicha ish yuritmoqda: Beeline, Mobi.uz, Ucell, UzMobile, Humans.",
      visible: false
   },
   {
      questinary: "Mobil qurilmaning IMEI-kodi holati qanday tekshiriladi?",
      answer: "Mobil qurilmaning IMEI-kodi holatini quyidagicha tekshirish mumkin: 1.UZIMEI tizimi operatorining ",
      visible: false
   },
   {
      questinary: "Mobil qurilmaning IMEI-kodi/kodlarini qanday bilish mumkin?",
      answer: "Qurilma klaviaturasida *#06# kombinatsiyasini kiritib, mobil qurilmaning IMEI-kodini/kodlarini bilib olish mumkin. Bundan tashqari, ushbu kod qurilmani qutisida, kafolat kartasida va ayrim qurilmalarni batareyasi ostida yozilgan bo‘ladi.",
      visible: false
   }
])
</script>

<template>
   <div class="container">
      <h2 class="text-center mb-10">Ko'p so'raladigan savollar</h2>
      <div class="flex justify-center items-center ">
         <div class="max-w-[840px]">
            <div v-for="item in _items" :key="item.questinary" @click="item.visible = !item.visible"
               class="px-5 cursor-pointer bg-white shadow-[0px_1.5px_6px_rgba(0,0,0,0.25)] rounded-lg py-3 my-5 flex justify-between"
               :class="item.visible && 'bg-primary/20 shadow-none'">
               <div>
                  <p class="font-sm font-poppins-700">{{ item.questinary }}</p>
                  <p v-if="item.visible" class="text-xs my-4">{{ item.answer }}</p>
               </div>
               <i :class="item.visible && 'rotate-180'" class="h-8 font-poppins-800 text-2xl ri-arrow-down-s-line"></i>
            </div>
         </div>
      </div>
   </div>

</template>