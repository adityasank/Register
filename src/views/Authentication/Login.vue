<template>
 <div class="authentication-bg">
  <vs-row vs-justify="center" class= " mt-5" >
    <vs-col type="flex" vs-w="6">
      <vs-card class="logincard">
        <vs-row>
          <vs-col vs-type="flex" class="section1" vs-justify="center" vs-align="center" vs-w="6">
            <vs-image class="loginimage" src=" img/login.png " />
          </vs-col>
          <vs-col vs-w="6">
            <div class="login ml-4 mr-4 mb-4">
              <h4 class="content1 mt-5">
                <b>Login</b>
              </h4>

              <h6 class="content2 mt-3">Welcome Back Please Login To your Account</h6>
              <vs-input
              icon="email"
                label-placeholder="Email"
                class="email mt-4"
                v-model="value1"
                icon-no-border
              />
              <vs-input   icon="vpn_key" type="password" label-placeholder="Password" class="mt-4"  icon-no-border v-model="value1" />
            </div>
            <vs-row>
              <vs-col vs-w="6">
                <vs-checkbox class="float-left ml-4" v-model="checkBox1">Remember Me</vs-checkbox>
              </vs-col>
              <vs-col vs-w="6">
                <p class="forgotpw float-right mr-4">Forgot Password</p>
              </vs-col>
            </vs-row>

            <vs-button class="register ml-4" color="primary" type="border">Register</vs-button>
            <vs-button class="loginbutton float-right mr-4" color="blue" type="filled">Login</vs-button>
            <div class="ml-4 mr-4">
              <hr />
              <div class = " mt-4 mb-4">
              <vs-button class= " facebook mr-2" color="#1551b1" type="filled"><i class="fa fa-facebook" width=" 20px" /></vs-button>
              <vs-button class= "twitter mr-2" color="#00aaff" type="filled"><i class="fa fa-twitter" width=" 20px" /></vs-button>
              <vs-button class= "google mr-2" color="#4285F4" type="filled"><i class="fa fa-google" width=" 20px" /></vs-button>
              <vs-button class= "github mr-2" color="#333333" type="filled"><i class="fa fa-github-alt" width=" 20px" /></vs-button>
<vs-button class= "auth float-right" color="#Eb5424" type="filled">Auth0</vs-button>
</div>
            </div>
          </vs-col>
        </vs-row>
      </vs-card>
    </vs-col>
  </vs-row>
 </div>
</template>
<style>
.vs-con-input-label {
  width: unset !important;
}
.vs-image--img{
  background-repeat: no-repeat;
}
.vs-card--content {
  padding: 0px !important;
  border-radius: 1px !important;
}
.logincard {
  font-family: Montserrat, Helvetica, Arial, sans-serif !important;
  margin-left: -70px;
  width: 120% !important;
  margin-top: 30px;
  border-radius: 0px !important;
}
.authentication-bg{
  background-image: url(/images/bg-pattern-light.svg);
	background-size: cover;
	background-position: center

}

</style>
<style scoped>
.section1 {
  background: #eff2f7;
}

.loginimage {
  width: 100%;
}
.content1 {
  font-size: 18px;
}
.content2 {
  font-size: 14px;
}
.register {
  padding-right: 30px;
  padding-left: 30px;
}
.loginbutton {
  padding-right: 30px;
  padding-left: 30px;
  background: #7367f0 !important;
}
.facebook ,.google, .github, .twitter{
  padding-left: 15px;
  padding-right: 15px;
}
</style>

<script>
export default {
  data() {
    return {
      checkBox1: false
    };
  }
};
</script>