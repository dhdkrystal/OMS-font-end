<template>
	<div>
		<el-container>
			<searchbar :showContent='"请输入要查询的资源名称"'></searchbar>
			<el-main class="maincontent" style="margin-top: 105px;">
				<div class="source-title">
					<el-row>
					  <el-col :span="12"><div class="grid-content">资源名称</div></el-col>
					  <el-col :span="12"><div class="grid-content">所属任务</div></el-col>
				  </el-row>
				</div>
				<div class="source-item"v-for="item in sourcelist">
				<el-row>
					<el-col :span="12"><div class="grid-content">{{item.name}}</div></el-col>
					<el-col :span="12"><div class="grid-content">{{item.task}}</div></el-col>
				</el-row>
				</div>
			</el-main>
		</el-container>
	</div>
</template>
<script>
export default {
  name: 'source-page',
  data () {
    return {
      sourcelist: [{name: '需求规格说明书模板', task: '智能外包管理平台'}, {name: '虹软人脸识别API使用手册', task: '智能外包管理平台'}, {name: '详细设计说明书模板', task: '智能外包管理平台'}, {name: '代码规范', task: '智能外包管理平台'}]
    }
  }
}
</script>
<style>
.source-title{
  padding:5px 0;
  height:20px;
  background-color: #d3dce6;
  margin-bottom: 10px;
}
.source-item{
	padding:20px 0;
  border: 1px solid #eee;
  margin-bottom: 10px;
}
.source-item:hover{
	padding:20px 0;
  border: 1px solid #e51c23;
  margin-bottom: 10px;
}
.el-col {
  	padding-left: 10px;
}

.grid-content {
  border-radius: 4px;
  min-height: 36px;
}

</style>