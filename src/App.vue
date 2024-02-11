<script setup>
import TopBar from './components/TopBar.vue'

import Body from './components/Body.vue'
import { inject } from '@vercel/analytics';

</script>

<template>
  <div>
     <header class="flex">
         <TopBar></TopBar>
     </header>
     <main class="flex">
 
       <div class="w-full">
         <Body></Body>
       </div>
       
     </main>
  </div>

  <inject></inject>
 </template>
 

<style scoped>

</style>
