<template>
  <div class="details-page">
  <div class="top">
    <h3>调拨信息详情</h3>
    <ul>
      <li>调拨单编号：2018062214331254</li>
      <li>创建时间：2018-06-01 00：00</li>
      <li>完成时间：</li>
    </ul>
    <ul>
      <li>调拨单状态：<b>待确认</b></li>
      <li>确认时间：</li>
      <li></li>
    </ul>
  </div>



  <div class="center">
      <h3>物资信息</h3>
      <div class="center-box">
      <el-table
      :data="tableData"
      style="width: 100%;">
      <el-table-column
        prop="date"
        label="物资名称"
        width="180">
      </el-table-column>
      <el-table-column
        prop="name"
        label="计量单位"
        width="80">
      </el-table-column>
      <el-table-column
        prop="address"
        label="调拨数量">
      </el-table-column>
      <el-table-column
      prop="address"
      label="单价（元）">
        </el-table-column>
        <el-table-column
        prop="address"
        label="总价（元）">
      </el-table-column>
      <el-table-column
      prop="address"
      label="交货期">
    </el-table-column>
    <el-table-column
    prop="xinxi"
    label="收货信息">
    </el-table-column>
    </el-table>
  </div>


  <p>采购单位：北京市建筑东城有限公司</p>
  <p>&nbsp;&nbsp;&nbsp;供应商：合同中统一能上名称</p>
  <p>备注信息：</p>

  </div>

<div class="bottom">
  <p>数量总计： <span>600</span></p>
  <p>物资总金额（元）: <b>￥10,600</b></p>
</div>



<el-button type="info" plain class='ljy-btn'>信息按钮</el-button>



</div>
</template>

<script>

  export default {
    name:'f-details',
    data() {
      return {
        tableData: [{
          date: '2016-05-02',
          name: '王小虎',
          address: '1518 ',
          xinxi:'查看'
        }, {
          date: '2016-05-04',
          name: '王小虎',
          address: '1517 ',
          xinxi:'查看'
        }]
      }
    }
  }

</script>

<style scoped>

  .top{
    width: 100%;
    height: 125px;
    border:1px solid #ccc;
    box-sizing: border-box;
  }

  h3{
    font-size: 15px;
    font-weight: 600;
    margin-left: 15px;
    margin-top: 15px;
  }

  ul{
    list-style: none;
    width: 100%;
    height: 43px;
    line-height: 43px;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }

  ul li{
    flex: 1;
    margin-left: 15px;
    font-size: 15px;
  }

  .center{
    width: 100%;
    height: 300px;
    border:1px solid #ccc;
    box-sizing: border-box;
    margin-top: 15px;
  }

  .cell{
    text-align: center;
  }

  .center-box{
    margin:0 15px;
  }

  .xinxi{
    cursor: pointer;
  }

  .center p{
    margin-top: 15px;
    margin-left: 15px;
  }

  .bottom{
    width: 100%;
    height: 120px;
    background: #eee;
    margin-top: 15px;
  }

  .bottom p{
    width: 100%;
    padding-top: 25px;
    text-align: right;
  }

  .bottom span{
    display: inline-block;
    width: 65px;
    margin-right: 15px;
  }

  .bottom b{
    margin-right: 15px;
    color:#f00;
  }

  .ljy-btn{
    float: right;
    margin-top: 15px;
    margin-bottom: 32px;
  }
</style>