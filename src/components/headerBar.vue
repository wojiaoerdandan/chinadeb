<template>
  <div class="header-bar">
    <p class='header-msg'>{{msg}}</p>
    <ul class="header-ul">
      <li v-for="(i,index) in linkList" :key="index">{{i.title}}</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name:'headerBar',
    data() {
      return {
        msg:'欢迎登陆 内蒙古能源发电投资集团有限公司供应链管理平台！',
        linkList:[
          {title:'工作台', path:'xxx', component:'xxx'},
          {title:'采购', path:'xxx', component:'xxx'},
          {title:'供应商', path:'xxx', component:'xxx'},
          {title:'物料', path:'xxx', component:'xxx'},
          {title:'销售', path:'xxx', component:'xxx'},
          {title:'商城', path:'xxx', component:'xxx'},
          {title:'财务', path:'xxx', component:'xxx'},
          {title:'经营分析', path:'xxx', component:'xxx'},
          {title:'企业认证', path:'xxx', component:'xxx'},
          {title:'系统', path:'xxx', component:'xxx'},
        ]
      }
    }
  }
</script>

<style>
  .header-bar{
    width: 100%;
    height: 120px;
    background:#1B2B8D;
  }

  .header-msg{
    text-align: center;
    line-height: 80px;
    color:#fff;
  }

  .header-ul{
    list-style: none;
    width: 80%;
    height: 50px;
    margin:-10px auto 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color:#fff;
  }

  .header-ul li:hover {
    color:#f0f;
    cursor: pointer;
  }



</style>