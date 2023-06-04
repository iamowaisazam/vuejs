<script>

 import {RouterView } from 'vue-router'
 import Header from './components/Header.vue';
 import Footer from './components/Footer.vue';

  export default {

    data() {
      return {
        count: 1
      }
    },
    components: {
      Header,
      Footer

    },
    mounted() {
  
      console.log(this.count)
      this.count = 2
      
    }
  }

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
    
  }

</style>