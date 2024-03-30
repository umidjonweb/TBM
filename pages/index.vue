<script lang="ts" setup>
 import Main from './main.vue'
 import Servic from './servic.vue'
 import Interactive from './interactive.vue'
 import NewsHome from './news-home.vue'
 import AboutUs from './aboutUs.vue'
 import Questinary from './questinary/index.vue'
 import Feedback from './feedback/about.vue'
</script>

<template>
   <NuxtLayout>
      <Main />
      <Servic />
      <Interactive />
      <NewsHome />
      <AboutUs />
      <Questinary />
      <Feedback />
   </NuxtLayout>
</template>