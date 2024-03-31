<template>
  <div class="container mx-auto">
    <div class="pt-[70px]">
      <h4 class="text-center mb-[50px]">Bo'limlar</h4>
      <div class="flex flex-wrap gap-[30px]">
        <div
          class="departmants__card flex gap-[20px] mt-8 w-full rounded-[25px] borde border-black border-opacity-10 p-[15px]"
          v-for="n of 6"
          :key="n"
        >
          <img
            src="@/assets/img/leader1.png"
            alt="departments"
            class="h-full object-cover w-[350px] rounded-[10px] "
          />
          <div class="pt-5 flex flex-col justify-between pl-5">
            <h3 class="text-bl">Komplaens nazorati bo'limi</h3>

            <p class="ext-black text-lg">
              Bo'lim boshlig'i : Rustamov Gani Xudoyarovich
            </p>
            <p class="ext-black text-lg">Telefon : (71) 240-07-24</p>
            <p class="ext-black text-lg">Email : g.rustamov@rtmc.uz</p>

            <nuxt-link to="#" class="w-[200px] py-[10px] rounded-[6px] hover:bg-bl/70 hover:text-white text-bl text-center border border-bl"> Batafsil </nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script></script>
<style>
.departmants__card {
  width:100%;
  height: 350px;
  box-shadow: 0px 0px 20px rgba(24, 47, 67, 0.2);
  padding: 35px;
}
</style>
