<script setup>
 import {RouterView } from 'vue-router'
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
 

 

</script>

<template>

   <Header/>
  <div class="content">
    <RouterView />
  </div>

   <Footer/>
</template>

<style scoped>

  .content{
    border: 1px solid;
  }

</style>