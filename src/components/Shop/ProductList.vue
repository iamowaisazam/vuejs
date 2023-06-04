
<script setup >
 import { RouterLink } from 'vue-router';
 import products from '../../services/products';


</script>
<template>
   
    <div class="product-list pt-3">
        <div class="container">
            <div class="row">
                <div v-for="item in products" class="col-md-3">
                    <div class="product">
                        <div class="image-wrapper">
                            <img :src="item.image" />
                        </div>
                        <div class="main-wrapper">
                            <span class="category" >{{item.category}}</span>
                            <RouterLink :to="'product/'+item.id" >
                                <h4 class="title" >{{item.title}}</h4>
                            </RouterLink>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped >

.product{
    border: 1px solid #ebebeb;
    padding: 10px;
    margin: 15px 0px;
}

.product img{
    width: 100%;
}

.product .category{
    color: #a9a9a9;
    text-transform: uppercase;
    font-size: .929em;
}

.product .title{
    color: #222;
    display: block;
    font-size: 1em;
    padding: 5px 0px;
    font-weight: 400;
}


</style>