<script setup>
import Bread from '../components/Bread.vue';
import {useRoute} from 'vue-router';
import products from '../services/products';


const route = useRoute();
const product = products.find( p => p.id == parseInt(route.params.id));

console.log(product);


</script>
<template>
    <Bread/>
    <div class="product-detail">
        <div class="container">
    
            <div class="product">
                <div class="container">
                    <div class="row">
                        <div class="col-md-6 mx-auto">
                             <div class="image-wrapper">
                                    <img src="http://sinrato.mallthemes.com/wp-content/uploads/2018/12/product15-400x400.jpg" />
                             </div>
                        </div>
                        <div class="col-md-6 mx-auto">
                            <div class="product">
                                
                                <div class="main-wrapper text-left">
                                        <span class="category">{{product.category ? product.category : ''}} </span>
                                        <h4 class="title" >{{product.title ? product.title : ''}}</h4>
                                        <p>
                                            <span class="new_price" >£50.00</span>
                                            <span class="old_price" ><del>£60.00</del></span>
                                        </p>
                                        <hr>
                                        <p>{{product.description ? product.description : ''}} </p>

                                        <div class="feature-list">
                                            <div class="item">
                                                <span class="label" >Ex Tax:</span>
                                                <span>£60.24</span>
                                            </div>
                                            <div class="item">
                                                <span class="label">Brands :</span>
                                                <span>Canon</span>
                                            </div>
                                            <div class="item">
                                                <span class="label">Product Code :</span>
                                                <span>Digital</span>
                                            </div>
                                            <div class="item">
                                                <span class="label">Reward Points :</span>
                                                <span>200</span>
                                            </div>
                                            <div class="item">
                                                <span class="label">Availability :</span>
                                                <span>In Stock</span>
                                            </div>

                                        </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>
<style scoped >

.product-detail{
    padding-bottom: 15px;
}

.image-wrapper{
    border:  1px solid lightgray;
    text-align: center;
}

.new_price{
    color: #fe4f19;
    font-size: 18px;
    font-weight: 600;
    padding-right: 5px;
    padding-top: 15px;

}

.product{
   padding-top: 10px; 
}


.label{
    color: black;
    font-weight: 500;
    padding-right: 5px;
}


</style>