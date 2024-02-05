<script setup>
import TopBar from './components/TopBar.vue'
import Footer from './components/Footer.vue'
import RightBar from './components/RightBar.vue'
import LeftBar from './components/LeftBar.vue'
import Body from './components/Body.vue'

</script>

<template>
  <div>
     <header class="flex items-center justify-center">
         <TopBar></TopBar>
     </header>
     <!-- Body -->
     <main class="flex flex-col md:flex-row m-2">
 
       <div class="flex-none w-full md:w-14 h-14">
         <RightBar />
       </div>
   
       <div class="grow h-14 body">
         <Body></Body>
       </div>
   
       <div class="flex-none w-full md:w-14 h-14">
         <LeftBar />
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
