<script lang="ts" setup>

const value = ref('')

const options = [
   {
      value: 'uz',
      label: "O'zbek",
   },
   {
      value: 'cr',
      label: 'Ўзбек',
   },
   {
      value: 'ru',
      label: 'Русский',
   }
]
</script>

<template>
   <header>
      <div class="container">
         <div class="flex justify-between items-center">
            <div class="flex gap-4">
               <a href="#">
                  <i class="ri-mail-fill"></i>
                  <span class="ml-2 text-black/80">tmc@rtmc.uz</span>
               </a>
               <a href="">
                  <i class="ri-phone-fill"></i>
                  <span class="ml-2 text-black/80">(71) 240-27-72
                  </span>
               </a>
               <a href="">
                  <i class="ri-phone-fill"></i>
                  <span class="ml-2 text-black/80">
                     (71) 240-54-19
                  </span>
               </a>
               <a href="">
                  <i class="ri-phone-fill"></i>
                  <span class="ml-2 text-black/80">1192</span>
               </a>
            </div>
            <el-select v-model="value" placeholder="" style="width: 100px">
               <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value" />
            </el-select>
         </div>
         <div class="flex justify-between items-center mt-4">
            <img @click="$router.push('/')" class="h-9 cursor-pointer" src="@/assets/img/logo.svg" />
            <div class="flex justify-between items-center">
               <div class="flex gap-6">
                  <a class="text-sm  text-black/90" href="">BOSH SAHIFA</a>
                  <a class="text-sm  text-black/90" href="">MARKAZ HAQIDA </a>
                  <a class="text-sm  text-black/90" href="">YANGILIKLAR</a>
                  <a class="text-sm  text-black/90" href="">KOMPLAENS</a>
                  <a class="text-sm  text-black/90" href="">HUJJATLAR</a>
                  <a class="text-sm  text-black/90" href="">QAYTA ALOQA</a>
                  <a class="text-sm  text-black/90" href="">poppinsAKTIV XIZMATLAR</a>
               </div>
               <div class="border-l pl-6 ml-4">
                  <i class="ri-search-line font-poppins-900 cursor-popoppins text-xl"></i>
               </div>
            </div>
         </div>
      </div>
   </header>

</template>
<style>
header {
   position: sticky;
   top: -1px;
   left: 0;
   background-color: #fff;
   z-index: 9;
   box-shadow: 0px 0px 10px rgba(24, 47, 67, 0.1);
   background-image: url(../assets/img/background-pattern.png);
   padding: 6px 0;
   padding-bottom: 11px;
}
</style>
