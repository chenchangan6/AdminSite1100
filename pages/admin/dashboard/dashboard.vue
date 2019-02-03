<template>
  <el-container class="main_container">
    <el-aside width="200px">
      <div class="side">
        <div class="logo-all">
          <img src="@/assets/images/logo/logo-1.png" />
        </div>
        <div class="main_menu">
          <el-menu name='mainMenues'
                   unique-opened
                   background-color="transparent"
                   text-color="#fff"
                   active-text-color="#ffd04b">
            <label v-for="x,index in MainMenu">
              <!-- 导航类 -->
              <label v-if="x.mode==='1'">
                <el-submenu :index="index+''">
                  <template slot="title">
                    <i :class="'icon font_family '+ x.icon"></i>
                    <span>{{x.title}}</span>
                  </template>
                  <label v-if="x.children.length">
                    <label v-for="y,z in x.children">
                      <el-menu-item :index="index+'-'+z">
                        <i :class="'icon font_family '+y.icon"></i>
                        <span slot="title">{{y.title}}</span>
                      </el-menu-item>
                    </label>
                  </label>
                </el-submenu>
              </label>
              <!-- 导航项 -->
              <label v-else-if="x.mode==='2'">
                <el-menu-item :index="index+''">
                  <i :class="'icon font_family '+x.icon"></i>
                  <span slot="title">{{x.title}}</span>
                </el-menu-item>
              </label>

            </label>
          </el-menu>
        </div>
      </div>

    </el-aside>
    <el-container>
      <el-header class="main_header">
        <el-row class="cor">
          <el-cor :span="2">
            <i class="icon font_family icon-shouqi"></i>
          </el-cor>
          <el-cor :span="2">
            <div>1</div>
          </el-cor>
          <el-cor :span="2">2</el-cor>
          <el-cor :span="2">3</el-cor>
          <el-cor :span="2">4</el-cor>
        </el-row>

      </el-header>
      <el-main class="main_main">Main</el-main>
    </el-container>
  </el-container>

</template>

<script>
export default {
  data() {
    return {
      MainMenu: [
        {
          MenuType: "Top",
          parentid: "0",
          title: "工作台",
          number: "1",
          icon: "icon-gongzuotai",
          mode: "2"
        },
        {
          MenuType: "Top",
          title: "课程管理",
          number: "1",
          icon: "icon-kechengguanli",
          mode: "1",
          children: [
            {
              MenuType: "Child",
              parentid: "1",
              title: "课程列表",
              number: "1",
              icon: "icon-kechengguanli",
              mode: "2"
            },
            {
              MenuType: "Child",
              parentid: "1",
              title: "课程分类",
              number: "1",
              icon: "icon-kechengguanli",
              mode: "2"
            }
          ]
        },
        {
          MenuType: "Top",
          title: "订单管理",
          number: "1",
          icon: "icon-dingdanguanli",
          mode: "1",
          children: [
            {
              MenuType: "Child",
              parentid: "2",
              title: "购买订单",
              number: "1",
              icon: "icon-dingdanguanli",
              mode: "2"
            },
            {
              MenuType: "Child",
              parentid: "2",
              title: "邀请订单",
              number: "1",
              icon: "icon-dingdanguanli",
              mode: "2"
            },
            {
              MenuType: "Child",
              parentid: "2",
              title: "积分兑换",
              number: "1",
              icon: "icon-dingdanguanli",
              mode: "2"
            },
            {
              MenuType: "Child",
              parentid: "2",
              title: "实物订单",
              number: "1",
              icon: "icon-dingdanguanli",
              mode: "2"
            }
          ]
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "打卡管理",
          number: "1",
          icon: "icon-daqiaguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "用户管理",
          number: "1",
          icon: "icon-yonghuguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "讲师管理",
          number: "1",
          icon: "icon-jiangshiguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "班级管理",
          number: "1",
          icon: "icon-banjiguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "视频管理",
          number: "1",
          icon: "icon-shipinguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "评价管理",
          number: "1",
          icon: "icon-pingjiaguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "消息管理",
          number: "1",
          icon: "icon-xiaoxiguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "积分管理",
          number: "1",
          icon: "icon-jifenguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "兑换码管理",
          number: "1",
          icon: "icon-duihuanmaguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "反馈管理",
          number: "1",
          icon: "icon-fankuiguanli",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "基本设置",
          number: "1",
          icon: "icon-jifenshezhi",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "管理员",
          number: "1",
          icon: "icon-guanliyuan",
          mode: "2"
        },
        {
          MenuType: "Top",
          parentid: "1",
          title: "数据统计",
          number: "1",
          icon: "icon-shujutongji",
          mode: "2"
        }
      ]
    };
  },
  layout: "admin"
};
</script>

<style>
</style>
