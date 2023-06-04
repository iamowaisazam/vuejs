<script setup>
import { RouterLink } from 'vue-router';


</script>
<template>
        <section class="desktop-menu " >
                <div class="container">
                    <div class="row">
                        <div class="img col-sm-12 col-md-6 text-sm-center text-md-start">
                           <RouterLink to="/" >
                            <img src="https://htmldemo.net/sinrato/sinrato/assets/img/logo/logo-sinrato2.png" 
                            alt="" />
                           </RouterLink>
                        </div>
                        <div class="col-sm-12 col-md-6 ">
                            <div class="menu-items" >
                                <div class="cart">
                                    <a class="ha-toggle" >
                                    <img src="https://fonts.gstatic.com/s/i/short-term/release/materialsymbolsoutlined/favorite/wght200/48px.svg" />
                                    </a>
                                </div>
                                <div class="cart">
                                    <a class="ha-toggle" >
                                    <img src="https://fonts.gstatic.com/s/i/short-term/release/materialsymbolsoutlined/shopping_bag/wght200/48px.svg" /></a>
                                </div> 
                                <div class="cart">
                                    <a class="ha-toggle" >
                                    <img src="https://fonts.gstatic.com/s/i/short-term/release/materialsymbolsoutlined/menu/wght200/48px.svg" /></a>
                                </div> 
                            </div>        
                        </div>
                    </div>
                </div>
            </section>
 
      
</template>


<style scoped >

        .desktop-menu{
                /* background: #fedc19; */
                padding: 25px 0px;
        
        }
    
    
    
    .menu-items {
        display: flex;
        /* justify-content: end; */
           
    }
    
    .menu-items a{
        text-decoration: none; 
        /* padding: 0px 5px; */
        margin: 0px 3px;
        color: white;
    }
    
    .menu-items a img{
        width: 40px;
    }
    
    
    @media (min-width: 400px) { 
        .menu-items{
     display: flex;   
     justify-content: center;
    }
    
    .desktop-menu{
        background: #fedc19;
        padding: 25px 0px;
       
    }
    .desktop-menu .img{
        text-align: center;
    }
    .desktop-menu .menu-items {
        display: flex;
        /* justify-content: end; */
        margin-top: 5px;
           
    }
     }
    /* // Small devices (landscape phones, 576px and up) */
    @media (min-width: 576px) { 
        .menu-items{
     display: flex;   
     justify-content: center;
    }
    
    .desktop-menu{
        background: #fedc19;
        padding: 25px 0px;
       
    }
    .desktop-menu .menu-items {
        display: flex;
        /* justify-content: end; */
        margin-top: 5px;
           
    }
     }
    
    /* // Medium devices (tablets, 768px and up) */
    @media (min-width: 768px) { 
        .desktop-menu{
            background: white;
            padding: 25px 0px;
           
        }
        .menu-items{
     display: flex;  
     justify-content: end; 
    }
    .desktop-menu .desktop-items{
      
        padding: 25px 0px;
       
    }
    .menu-items {
        display: flex;
        /* justify-content: end; */
           
    }
    
     }
    
    /* // Large devices (desktops, 992px and up) */
    /* @media (min-width: 992px) { ... } */
    
    /* // X-Large devices (large desktops, 1200px and up) */
    /* @media (min-width: 1200px) { ... } */
    
    /* // XX-Large devices (larger desktops, 1400px and up) */
    /* @media (min-width: 1400px) { ... } */

</style>