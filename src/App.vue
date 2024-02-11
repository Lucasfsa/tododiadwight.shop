<script setup>
import TopBar from './components/TopBar.vue'
import Footer from './components/Footer.vue'
import RightBar from './components/RightBar.vue'
import LeftBar from './components/LeftBar.vue'
import Body from './components/Body.vue'

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
<!--  
     <footer>
         <Footer></Footer>
     </footer> -->
 
  </div>
 </template>
 

<style scoped>

</style>
