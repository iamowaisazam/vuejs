
<script setup >
   
    import { useRouter } from 'vue-router';
    import Bread  from '../components/Bread.vue';
    import {getUsers} from '../services/users';
    
    let form = {
        email:"",
        password:"",
    }

    const route = useRouter();
    const register = () => {

        // let users = getUsers();
        // let email = users.find( u => u.email == form.email);
        // let password = users.find( u => u.password == form.password);

        // if(email == undefined || password == undefined){
        //         alert("Invalid Details");
        //         return false;
        // }

        alert("Registration Success Now You Can Loggedin");
        route.push("/login");

    }

</script>
  <template>
      <Bread />
       
      <section class="login-section" >
        <div class="container">
            <div class="row">
                <div class="col-md-6 mx-auto">
                    <div class="section-title">
                        <h3 class="title" >Register To Your Account</h3>
                    </div>

                    <div class="login-form">
                        <div class="container">
                        <form action="">
                            <div class="row">
                                <div class="col-md-12">
                                    <label class="label" >Email</label>
                                    <input class="form-control" type="text" v-model="form.email" />
                                </div>
                            </div>
                            <div class="row pt-3">
                                <div class="col-md-12">
                                    <label class="label" >Password</label>
                                    <input class="form-control" type="text" v-model="form.password" />
                                </div>
                            </div>
                            <div class="row">
                                <div class="col-md-12  text-center py-3">
                                    <button type="button" @click="register" class="btn btn-primary" >Submit</button>
                                </div>
                            </div>
                            <!-- <hr> -->
                            <div class="row">
                                <div class="col-md-12 text-center">
                                    <RouterLink class="redirect_link" to="/login">If You Already Have Account ?</RouterLink>
                                </div>
                            </div>

                         </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
      </section>
      
 </template>
  
  <style scoped >

    .redirect_link{
        text-decoration: none;
        margin: 0;
        padding: 0;
        color: #444;
        font-size: 14px;
        font-weight: 400;
        line-height: 24px;
    }

    .login-section{
        padding-bottom: 30px;
    }

  .login-form{
      border: 1px solid lightgray;
      padding: 25px 10px 16px 10px;

  }

  .label{
    padding-bottom: 15px;
  }

  .title{
    background: #fff none repeat scroll 0 0;
    color: #111;
    display: inline-block;
    font-size: 26px;
    padding-right: 30px;
    position: relative;
    text-transform: capitalize;
    text-align: center;
  }

  .section-title {
    position: relative;
    margin-top: 54px;
    margin-bottom: 22px;
    text-align: center;
    }

    .section-title::after {
        background: #f0f0f0;
        content: "";
        height: 1px;
        position: absolute;
        top: 50%;
        width: 100%;
        left: 0;
        z-index: -1;
    }

  </style>
  