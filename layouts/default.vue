<template>
  <div>
    <div class="dev-nav">
<ul class="dev-nav">
  <li><nuxt-link to="/login">后台登陆页面</nuxt-link></li>
  <li><nuxt-link to="/singUp/teacher/singUp">讲师注册页面</nuxt-link></li>
  <li><nuxt-link to="/singUp/teacher/addInfo">完善信息</nuxt-link></li>
  <li><nuxt-link to="/singUp/teacher/finish">完成注册</nuxt-link></li>
  <li><nuxt-link to="/admin/dashboard/dashboard">工作台</nuxt-link></li>

</ul>
    </div>
    <nuxt/>
  </div>
</template>
<script>
export default {
  data() {
    return {
      cc: 11
    };
  }
};
</script>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
