<template>
    <el-main class="maincontent">
       <el-row class="myEl-Row">
        <font class="el-rowText">合同信息</font>
      </el-row>
      <div style="height:40px"></div>
      <div style="height:60px">
        <span style="margin-left:2%;margin-right:5%;text-decoration:underline;font-weight:bold">合同信息</span>
        <el-button type="primary" round>修改</el-button>
      </div>

      <el-row class="myEl-Row">
        <font class="el-rowText">保密协议</font>
      </el-row>
      <div style="height:40px"></div>
      <div style="height:60px">
        <span style="margin-left:2%;margin-right:5%;text-decoration:underline;font-weight:bold">保密协议</span>
        <el-button type="primary" round>修改</el-button>
      </div>
    </el-main>

</template>
<script>
  export default {
    name: 'info',
    data () {
      return {
      }
    }
  }
</script>

