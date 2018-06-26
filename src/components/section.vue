<template>

  <div class="section">
    <div class='crumbs'>
      <div class="crumbs-box">
        <el-breadcrumb separator-class="el-icon-arrow-right">
          <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
          <el-breadcrumb-item>活动管理</el-breadcrumb-item>
          <el-breadcrumb-item>活动列表</el-breadcrumb-item>
          <el-breadcrumb-item>活动详情</el-breadcrumb-item>
        </el-breadcrumb>
      </div>
    </div> 


    <div class='tab'>
      <div class="tab-box">
        <el-tabs v-model="activeName">
          <el-tab-pane label="用户管理" name="first"><f-details></f-details></el-tab-pane>
          <el-tab-pane label="配置管理" name="second">配置管理</el-tab-pane>
          <el-tab-pane label="角色管理" name="third">角色管理</el-tab-pane>
          <el-tab-pane label="定时任务补偿" name="fourth">定时任务补偿</el-tab-pane>
        </el-tabs>
      </div>
    </div>



  </div>

</template>

<script>
  import Fdetails from './details'
  export default {
    name:'sections',
    data() {
      return {
        activeName: 'first'
      };
    },
    components: {
      "f-details":Fdetails,
    }
  }

</script>

<style>

  .section{
    width: 100%;
    height: 100%;
    background: #f2f2f2;
    float: right;
    margin-left: 30px;
  }

  .crumbs{
    width: 100%;
    height: 50px;
    background: #fff;
  }

  .crumbs-box{
    float: left;
    margin-top: 18px;
    margin-left: 15px;
  }

  .tab{
    background: #fff;
    margin-top: 15px;
  }
  .tab-box{
    margin:0 15px;
  }

</style>