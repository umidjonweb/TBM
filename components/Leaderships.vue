<template>
  <div class="container mx-auto">
    <div class="pt-[70px]">
      <h4 class="text-center mb-[50px]">Rahbariyat</h4>
      <div class="flex flex-wrap gap-[30px]">
        <div class="leadership__card rounded-[6px]" v-for="n of 6" :key="n">
          <img
            src="@/assets/img/leader1.png"
            alt="leader"
            class="w-full object-cover h-[145px]"
          />
          <div class="pl-[10px]">
            <h4 class="mt-9 mb-3">Shakirov Ulugbek Anvarovich</h4>
            <p class="font-poppins mb-3">Direktorning birinchi o`rinbosari</p>
            <div>
              <p class="font-popins">
                Telefon: +998 71&nbsp;240-27-72<br />Qabul kunlari: har oyning
                birinchi va oxirgi payshanba kunlari, 10:00 - 12:00<br />E-mail:&nbsp;tmc@rtmc.uz
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script></script>
<style>
.leadership__card {
  width: 370px;
  height: 530px;
  box-shadow: 0px 0px 20px rgba(24, 47, 67, 0.2);
  padding: 35px;
}
</style>
