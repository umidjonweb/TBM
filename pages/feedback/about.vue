<script lang="ts" setup>
const _item = ref({
   email: '',
   text: '',
})

</script>
<template>
   <div class="container !my-20">
      <h2 class="text-center">Qayta aloqa</h2>
      <p class="max-w-[500px] w-full mx-auto my-10">Bu yerda siz tizim operatori faoliyatiga oid sharh va mulohazalaringizni
         qoldirishingiz mumkin.</p>
      <div class="grid grid-cols-3 gap-4 max-w-[700px] mx-auto">
         <input placeholder="Elektron manzilingiz" class="border border-primary/30 rounded-lg" v-model="_item.email"
            type="email" />
         <input placeholder="Murojaat matni" class="border border-primary/30 rounded-lg" v-model="_item.text"
            type="email" />
         <button @click="$router.push({path: '/feedback', query: { item: JSON.stringify(_item)}})" class="bg-green text-white  rounded-lg flex gap-2 items-center justify-center ">
            <span>Biz bilan bog'lanish </span>
            <i class="text-xl ri-arrow-right-s-line"></i>
         </button>
      </div>
   </div>
</template>

<style lang="scss">
input {
   padding: 0px 16px;

   &::placeholder {
      color: #C4C8E1;
   }
}
</style>