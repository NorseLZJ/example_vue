<script setup lang="ts">
</script>

<template>
  <div class="common-layout">
    <el-container>
      <el-header class="h-header">Header</el-header>
      <el-main>

      <el-row :gutter="10" class="centered-row">
			  <el-col :span="5"><div class="grid-content ep-bg-purple"> 翻译 </div></el-col>
			  <el-col :span="5"><div class="grid-content ep-bg-purple"> 生成图片 </div></el-col>
			  <el-col :span="5"><div class="grid-content ep-bg-purple"> 生成分镜 </div></el-col>
			  <el-col :span="5"><div class="grid-content ep-bg-purple"> 生成音乐 </div></el-col>
		  </el-row>

      </el-main>
    </el-container>

    </div>
</template>

<style scoped>
.centered-row {
  display: flex;
  justify-content: center;
}
.h-header{
  background-color: blanchedalmond;
}

.el-row {
  margin-bottom: 10px;
}
.el-row:last-child {
  margin-bottom: 0;
}
.el-col {
  border-radius: 4px;
}

.grid-content {
  border-radius: 4px;
  min-height: 36px;
  height: 300px; /* 设置高度为100px */
  width: 300px; /* 设置宽度为100px，以确保是正方形 */
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(0, 128, 17);
  color: white;
}
</style>