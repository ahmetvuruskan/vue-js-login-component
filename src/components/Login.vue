<template>
<div>
  <div class="container-center-horizontal">
    <div class="dashboard-login-dark-theme screen">
      <div class="form">
        <h1 class="title">{{title}}</h1>
        <p class="sign-in-and-start-ma lexenddeca-normal-white-16px">{{text}}</p>
        <input class="login lexenddeca-normal-white-14px overlap-group2" :placeholder="login" >
        <input class="login lexenddeca-normal-white-14px overlap-group2" :placeholder="password" >

        <div class="section-forgot">
          <div class="rectangle-1"></div>
          <div class="remember-me">{{rememberMe}}</div>
          <div class="forgot-password">{{forgotPassword}}</div>
        </div>
        <button @click="log()" class="overlap-group login-1 lexenddeca-normal-white-16px">{{login}}</button>
        <div class="overlap-group3">

        </div>
      </div>
    </div>
  </div>

</div>
</template>


<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Login",
  props :['title','text','login','password','rememberMe','forgotPassword'],
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:500|Lexend+Deca:400');


.lexenddeca-normal-white-16px{
  color:white;
  font-family: 'Lexend Deca',serif;
  font-size: 16px;
  font-weight: 400;
  font-style: normal;
}
.lexenddeca-normal-white-14px{
  color:white;
  font-family: 'Lexend Deca',serif;
  font-size: 14px;
  font-weight: 400;
  font-style: normal;
}

.screen a{
  display: contents;
  text-decoration: none;

}
.container-center-horizontal{
  display: flex;
  flex-direction: row;
  justify-content: center;
  pointer-events: none;
  width: auto;
}
.container-center-horizontal>*{
  flex-shrink: 0;
  pointer-events: auto;
}
.dashboard-login-dark-theme {
  align-items: center;
  background-color: #093545;
  border: 1px none;
  display: flex;
  flex-direction: column;
  height: 850px;
  width:1500px;
}
.form{
  align-items: center;
  display: flex;
  flex-direction: column;
  margin-left: 3px;
  margin-top: 157px;
  min-height: 406px;
  width: 351px;
}
.title{
  color: rgba(255,255,255,1);
  font-family: 'Lexend Deca',serif;
  font-size: 64px;
  font-weight: 400;
  letter-spacing: 0;
  margin-right: 3px;
  min-height: 80px;
  min-width: 212px;
  text-align: center;
}
.sign-in-and-start-ma{
  letter-spacing: 0;
  margin-right: 4px;
  margin-top: 39px;
  min-height: 20px;
  min-width: 347px;
  text-align: center;
}
.overlap-group2{
  align-items: flex-start;
  background-color:rgba(34,73,87,1) ;
  border-radius: 10px;
  display: flex;
  height: 45px;
  margin-right: 3px;
  margin-top: 36px;
  min-width: 300px;
  padding: 12px 18px;
}
.login{
  letter-spacing: 0;
  line-height: 20px;
  min-height: 20px;
  min-width: 20px;
  text-align: center;
  white-space: nowrap;
}
.overlap-group1{
  align-items: flex-end;
  background-color:rgba(34,73,87,1) ;
  border-radius: 10px;
  display: flex;
  height: 45px;
  margin-right: 3px;
  margin-top: 32px;
  min-width: 300px;
  padding: 12px 21px;
}
.password{
  letter-spacing: 0;
  line-height: 20px;
  min-height: 20px;
  min-width: 65px;
  text-align: center;
  white-space: nowrap;
}
.section-forgot{
  align-items: flex-start;
  display: flex;
  margin-top: 23px;
  min-width: 297px;
}
.rectangle-1{
  background-color: rgba(34,73,87,1);
  border:1px none;
  border-radius: 5px;
  height: 17px;
  width: 18px;
}
.remember-me{
  color: white;
  font-family: 'Lexend Deca',serif;
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0;
  margin-left: 7px;
  min-height: 17px;
  min-width: 108px;
  text-align: left;
}
.forgot-password{
  color: #00cc99;
  font-weight: 500;
  letter-spacing: 0;
  margin-left: 32px;
  min-height: 17px;
  min-width: 128px;
  text-align: center;
}
.overlap-group {
  align-items: flex-end;
  background-color: #00cc99;
  border-radius: 10px;
  box-shadow: 0px 4px 4px #0000004c;
  display: flex;
  height: 45px;
  margin-right: 3px;
  margin-top: 24px;
  min-width: 300px;
  padding: 12px 128px;
}

.login-1{
  letter-spacing: 0;
  line-height: 20px;
  min-height: 20px;
  min-width: 44px;
  text-align: center;
  white-space: nowrap;
}
.overlap-group3{
  align-items: flex-end;
  display: flex;
  height: 111px;
  margin-top: 46px;
  min-width: 1280px;
  padding: 20px 36px;
}
.overlap-group-1{
  align-items: center;
  background-color: #2c2c2c;
  border-radius: 21.5px;
  display: flex;
  height: 43px;
  padding: 0 5px;
}
.ellipse-3{
  height: 33px;
  width: 17px;
}


</style>