<template>
<div>
<login
    :title="title"
    :text="text"
    :login="login"
    :password="password"
    :rememberMe ="rememberMe"
    :forgotPassword = "forgotPassword"
></login>
</div>

</template>

<script>
import Login from "@/components/Login";

export default {
  components:{
    login : Login
  },
  data : function (){
    return {
      title : "Sign in",
      text : "Sign in and managing your candidates!",
      login: "Login",
      password: "Password",
      rememberMe : "Remember Me",
      forgotPassword :"Forgot Password ? "
    }
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
