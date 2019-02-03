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
          <el-steps :active="2"
                    align-center>
            <el-step title="注册账号"></el-step>
            <el-step title="完善信息"></el-step>
            <el-step title="完成"></el-step>
          </el-steps>
        </div>
      </div>
      <div class="login-form">
        <el-form label-width="100px">
          <el-form-item label="姓名"
                        prop="pass">
            <el-input type="password"
                      autocomplete="off"></el-input>
          </el-form-item>
          <el-form-item label="头衔"
                        prop="checkPass">
            <el-input type="password"
                      autocomplete="off"></el-input>
            <div style="text-align:left;"><span>如：丹棱科技小院专家，柑橘种植专家等。</span></div>
          </el-form-item>

          <el-form-item label="头像"
                        prop="age">
            <div style="text-align:left;">
              <el-upload class="avatar-uploader"
                         action="https://jsonplaceholder.typicode.com/posts/">
                <img v-if="imageUrl"
                     :src="imageUrl"
                     class="avatar">
                <i v-else
                   class="el-icon-plus avatar-uploader-icon"></i>
              </el-upload>
            </div>
            <div style="text-align:left;"><span>请上传真人头像，JPG,PNG,文件小于1M.</span></div>
          </el-form-item>
          <el-form-item label="简介">
            <el-input type="textarea"
                      :rows="4"
                      placeholder="500字以内"
                      >
            </el-input>
          </el-form-item>
        </el-form>
      </div>
      <div style="margin:60px 30px;">
        <el-button style="width:360px;"
                   type="warning">提交</el-button>
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
