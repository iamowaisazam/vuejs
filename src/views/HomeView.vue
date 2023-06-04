<script setup >
import ProductList from '../components/Shop/ProductList.vue';
</script>
<template>

  <div class="container-fluid">
    <img class="img-fluid" src="https://htmldemo.net/sinrato/sinrato/assets/img/slider/slider1-home1.jpg" />
</div>

  <section class="top-rated-products" >
    <h3 class="text-center"> Top Rated Products</h3>
    <ProductList/>
  </section>


 
</template>

<style scoped >
.top-rated-products{
  margin: 50px 0px;
}


</style>