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
          <el-steps :active="3"
                    align-center>
            <el-step title="注册账号"></el-step>
            <el-step title="完善信息"></el-step>
            <el-step title="完成"></el-step>
          </el-steps>
        </div>
      </div>
      <div class="login-form" style="padding-left:100px">

        <i class="el-icon-success"></i>
        <div style="margin:30px 0px;font-size:20px;">
         信息提交成功！我们会尽快联系您！
        </div>
      </div>
      <div style="margin:60px 30px;">
        <el-button style="width:360px;"
                   type="warning">请马上联系我！</el-button>
      </div>
    </el-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pwd: "",
      usr: "",
      imageUrl: ""
    };
  },
  layout: "login"
};
</script>

<style>
</style>
