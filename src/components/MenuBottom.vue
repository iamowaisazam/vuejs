<script setup >
import { RouterLink } from 'vue-router';


</script>
<template>
    <div class="navigation">
        <div class="container">
            <div class="row">
                <div class="col-md-8 col-lg-6">        
                    <div class="menu">
                        <div class="item"><RouterLink to="/" >Home</RouterLink></div>
                        <div class="item"><RouterLink to="/shop" >Shop</RouterLink></div>
                        <div class="item"><RouterLink to="/" >Categories</RouterLink></div>
                        <div class="item"><RouterLink to="/" >Contact Us</RouterLink></div>   
                    </div>
                </div>
                <div class="contact-info col-md-4 col-lg-6 align-self-center">
                    <p class="m-0 text-end" ><span class="lnr lnr-phone"></span>Hotline : <strong>1-001-234-5678</strong></p>
                </div>
            </div>
        </div>
    </div>

</template>


<style scoped >
.navigation {
    background-color: #fedc19;
    /* display: block; */
}

/* .menu {
    display: flex;
    display: block;
} */

/* .menu .item {} */

.menu a {
    text-decoration: none;
    color: black;
    padding: 10px 15px;
    display: block;
}

.menu a:hover {
    background-color: black;
    color: white;
}


@media (min-width: 400px) {
    .navigation {
        background-color: #fedc19;
        display: block;
        text-align: center;
        overflow-y: auto;
       height: 300px;
       margin-bottom: 10px;
    }
    .navigation .contact-info{
        display: none;

    }
  
}
/* // Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
    /* .navigation {
        background-color: #fedc19;
        display: none;
    } */
}

/* // Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
    .navigation {
        background-color: #fedc19;
        display: block;
        text-align: center;
        overflow-y: auto;
        height: 45px;
        margin-bottom: 0px;
    }
    .menu {
        display: flex;
    }
    .navigation .contact-info{
        display: block;

    }

}

/* // Large devices (desktops, 992px and up) */
/* @media (min-width: 992px) { ... } */

/* // X-Large devices (large desktops, 1200px and up) */
/* @media (min-width: 1200px) { ... } */

/* // XX-Large devices (larger desktops, 1400px and up) */
/* @media (min-width: 1400px) { ... } */
</style>