<script setup >
import { RouterLink } from 'vue-router';
import { useCounterStore } from "../store/counter";

const store = useCounterStore();

console.log(store);
  
</script>
<template>
    <section class="topbar">
        <div class="container">
            <div class="row">
               <div class="left col-xs-12 col-md-7 col-lg-6 ">
                  <div class="d-flex justify-content-center  ">
                      <div class="item ">
                          <span class="light-text pe-2">Email:{{store.count}}</span>
                          <span @click="store.increament" >support@sinrato.com</span>
                      </div>
                      <span class="px-3" >|</span>
                      <div class="item">
                         <span>Free Shipping for all Order of $99</span>
                      </div>
                  </div>
               </div>
                <div class="right col-xs-12 col-md-5 col-lg-6  ">
                  <div class="menu-list">
                    <RouterLink to="/login">My Account</RouterLink>
                    <RouterLink to="/">Language</RouterLink>
                    <RouterLink to="/">Currency</RouterLink>
                  </div>
                </div>
            </div>
        </div>
      </section>
</template>
<style scoped>
.topbar{
    background-color: #222;
    padding: 10px 0px;
    color: white;
    font-size: 14px;
  }
  
  .row{
    display: flex;
    justify-content: space-between;
  }
  
  .light-text{
    color: #aaa;
  }
  
  .menu-list a{
    text-decoration: none;
    color: white;
    margin: 0px 5px;
  }
  
  .menu-list a:hover{
    color: #fedc19;
  }
  .topbar .left,
  .topbar .right{
  font-size: 13px;}
  
  
  
  
  
  @media (min-width: 400px) {
    .right {
       text-align: center;
    }
  }
  /* // Small devices (landscape phones, 576px and up) */
  @media (min-width: 576px) {
    .right {
       text-align: center;
    }
  }
  /* // Medium devices (tablets, 768px and up) */
  @media (min-width: 768px) { 
    .right {
      text-align: end;
   }
  
  }
  
  /* // Large devices (desktops, 992px and up) */
  /* @media (min-width: 992px) { ... } */
  
  /* // X-Large devices (large desktops, 1200px and up) */
  /* @media (min-width: 1200px) { ... } */
  
  /* // XX-Large devices (larger desktops, 1400px and up) */
  /* @media (min-width: 1400px) { ... } */

</style>