<template>
  <div class="singup">
    <el-card class="box-card">
      <div style="margin-top:20px;">
        <img src="@/assets/images/logo/logo-login.png"
             alt="新农人学社logo"
             class="logo">
      </div>
      <div style="margin-top:20px;margin-bottom:60px;">
        <div style="text-align:left;">
          <el-steps :active="1"
                    align-center>
            <el-step title="注册账号"></el-step>
            <el-step title="完善信息"></el-step>
            <el-step title="完成"></el-step>
          </el-steps>
        </div>
      </div>
      <div class="login-input">
      <div style="margin-bottom:20px;">
        <el-input v-model="usr"
                  placeholder="登陆名"></el-input>
      </div>
      <div style="margin-bottom:20px;">
        <el-input v-model="pwd"
                  placeholder="密码"></el-input>
      </div>
      </div>
      <div style="margin-bottom:40px;">
        <el-input style="width:235px; margin-right:10px;" placeholder="验证码"></el-input><el-button type="warning" plain>发送验证码</el-button>
      </div>
      <div style="margin-bottom:100px;">
        <el-button style="width:360px;"
                   type="warning">注册</el-button>
      </div>

    </el-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pwd: "",
      usr: ""
    };
  },
  layout: "login"
};
</script>

<style>
</style>
