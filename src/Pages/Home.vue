<script setup>
import Header from '@/components/Header.vue';
import Sidebar from '../components/Sidebar.vue'
import Test from '@/components/Test.vue';

</script>
<template>
   <div class="flex justify-between">
   <Sidebar/>
   <Header/>
   </div>
   <div class="flex justify-center"><Test/></div>
  
</template>
