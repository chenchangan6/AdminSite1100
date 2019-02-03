<template>
  <div class="singup">
    <el-card class="box-card">
      <div style="margin-top:30px;">
        <img src="@/assets/images/logo/logo-login.png"
             alt="新农人学社logo"
             class="logo">
      </div>
      <div style="margin-top:20px;margin-bottom:60px;font-size:30px;"><span>后台管理登陆</span></div>
      <div style="margin-bottom:20px;">
        <el-input v-model="usr"
                  placeholder="登陆名"></el-input>
      </div>
      <div style="margin-bottom:20px;">
        <el-input v-model="pwd"
                  placeholder="密码"></el-input>
      </div>
      <div style="text-align:left;padding-left:38px;margin-bottom:40px;">
        <el-checkbox v-model="savepwd"
                     text-color="#606266">记住密码</el-checkbox>
      </div>
      <div style="margin-bottom:40px;">
        <el-button style="width:360px;"
                   type="warning">登陆</el-button>
      </div>

    </el-card>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>
