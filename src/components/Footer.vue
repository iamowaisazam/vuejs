<script>

</script>
<template>
    <section class="footer">
        <div class="container">
            <div class="row">
                <div class="col-md-12 col-lg-6 col-xl-4 mb-5">
                    <RouterLink to="/">
                        <img class="logo" 
                           src="https://htmldemo.net/sinrato/sinrato/assets/img/logo/logo-sinrato.png" />
                    </RouterLink>
                    <p>We are a team of designers and developers that create high quality Magento, Prestashop, 
                        Opencart.</p>
                    <h6 class="sub-title" >Payment</h6>
                    <img src="https://htmldemo.net/sinrato/sinrato/assets/img/payment/payment.png" />
    
                </div>
                <div class="col-md-4 col-lg-6 col-xl-2">
                    <h4 class="title" >Information</h4>
                    <ul>
                        <li><a class="link-item"  href="about.html">About us</a></li>
                        <li><a class="link-item" href="#">Delivery Information</a></li>
                        <li><a class="link-item" href="#">Privacy Policy</a></li>
                        <li><a class="link-item" href="#">Terms &amp; Conditions</a></li>
                        <li><a class="link-item" href="#">Contact Us</a></li>
                        <li><a class="link-item" href="#">Returns</a></li>
                        <li><a class="link-item" href="#">Site Map</a></li>
                    </ul>
                </div>
                <div class="col-md-4 col-lg-6 col-xl-3">
                    <h4 class="title"  >Contact us</h4>
                    <ul>
                        <li><span>Address:</span> 4710-4890 Breckinridge St,Fayetteville, NC 28311</li>
                        <li><span>email:</span> support@sinrato.com</li>
                        <li><span>Call us:</span> <strong> 1-1001-234-5678</strong></li>
                    </ul>
                </div>
                <div class="col-md-4 col-lg-6 col-xl-3 d-md-block d-none" >
                    <h4 class="title"  >Our Twitter Feed</h4>
                    <div class="twitter-text">
                        Check out "Alice - Multipurpose Responsive #Magento #Theme" on #Envato by <a href="#">@sinratos</a> #Themeforest <a href="#">https://t.co/DNdhAwzm88</a>
                    </div>
                </div>
            </div>
        </div>
    
    
    </section>
</template>
<style scoped>
.footer{
    padding: 20px 10px;
}

.footer a{
    text-decoration: none;
    color: #444;
    
    
}


.footer .logo{
    padding: 20px 0px;
}

.footer p {
    color: #444;
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
}

.footer .sub-title{
    padding-bottom: 5px;
}



.footer .title{
    font-size: 18px;
    font-weight: 500;
    padding-bottom: 15px;
}

.footer ul a:hover{
 color: #ffc107;
    
}

.footer ul {
    list-style: none;
    color: #444;
    margin: 0px;
    padding: 0px;
}

.footer ul li {
    padding: 5px 0px;
    font-size: 14px;
}

.twitter-text {
    background: #f8f8f8;
    border: 1px solid #f0f0f0;
    border-radius: 7px;
    line-height: 24px;
    margin-bottom: 65px;
    padding: 20px;
    position: relative;
}
</style>