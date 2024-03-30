<script lang="ts" setup>
const _item = ref({
   fullName: "",
   email: "",
   department: "",
   feedback: ""
})
const options = [
   {
      value: 'Option1',
      label: 'Option1',
   },
   {
      value: 'Option2',
      label: 'Option2',
   },
   {
      value: 'Option3',
      label: 'Option3',
   },
   {
      value: 'Option4',
      label: 'Option4',
   },
   {
      value: 'Option5',
      label: 'Option5',
   },
]

</script>
<template>
   <NuxtLayout>
      <div class="container !my-20">
         <div class="grid grid-cols-2 gap-6 ">
            <div>
               <h2 class="my-6">Bog‘lanish</h2>
               <el-form label-position="top">
                  <el-form-item label="Ism va familiya">
                     <el-input size="large" v-model="_item.fullName" />
                  </el-form-item>
                  <el-form-item label="Elektron manzilingiz">
                     <el-input size="large" v-model="_item.email" />
                  </el-form-item>
                  <el-form-item label="Bo'limni tanlang">
                     <el-select size="large" v-model="_item.department" clearable placeholder="Bo'lim">
                        <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value" />
                     </el-select>
                  </el-form-item>
                  <el-form-item label="Nima uchun ariza beryapsiz??">
                     <el-input size="large" rows="4" type="textarea" placeholder="Murojaat matni"
                        v-model="_item.feedback" />
                  </el-form-item>

                  <el-form-item>
                     <button class="bg-green my-8 text-white w-full rounded-lg flex gap-2 items-center justify-center ">
                        <span>Bog'lanish </span>
                        <i class="text-xl ri-arrow-right-s-line"></i>
                     </button>
                  </el-form-item>
               </el-form>

            </div>
         </div>
         <div class="grid grid-cols-3 gap-6">
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">Manzil:</p>
               <p>O’zbekiston Respublikasi, Toshkent shahri, Olmazor tumani, 18-A uy, 240-ATS binosi</p>
            </div>
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">E-mail manzili</p>
               <p>mc@rtmc.uz, rtmc@exat.uz</p>
            </div>
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">Qabulxona:</p>
               <p>(998-71) 240-27-72</p>
            </div>
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">Telegram boti:</p>
               <p>@uztbmbot</p>
            </div>
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">Veb sayt:</p>
               <p>www.rtmc.uz</p>
            </div>
            <div class="border flex flex-col min-h-36 justify-center  border-green rounded py-6 pl-16 pr-6 ">
               <p class="font-poppins-700">Faks:</p>
               <p>(71) 240-54-19</p>
            </div>

         </div>
      </div>
   </NuxtLayout>
</template>

<style></style>