<script setup lang="ts">
</script>

<template>
  <div class="common-layout">
    <el-container>
      <el-header class="h-header">Header</el-header>
      <el-main>

        <el-row :gutter="11" class="centered-row">

          <el-col :span="6">
            <router-link to="/translation" class="grid-link">
              <div class="grid-content">
                <img src="./assets/1111.jpeg" alt="Translation">
                <span class="text-overlay">翻译</span>
              </div>
            </router-link>
          </el-col>

          <el-col :span="6">
            <div class="grid-content">
              <img src="./assets/2222.png" alt="Generate Image">
              <span class="text-overlay">生成图片</span>
            </div>
          </el-col>

          <el-col :span="6">
            <div class="grid-content">
              <img src="./assets/l3.jpeg" alt="Generate Storyboard">
              <span class="text-overlay">生成分镜</span>
            </div>
          </el-col>

          <el-col :span="6">
            <div class="grid-content">
              <img src="./assets/l4.jpeg" alt="Generate Music">
              <span class="text-overlay">生成音乐</span>
            </div>
          </el-col>

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

.h-header {
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
  height: 300px;
  width: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}

.grid-content img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 4px;
}

.text-overlay {
  position: absolute;
  top: 50%;
  /* 将文字的顶部定位在父容器的50%位置 */
  left: 50%;
  /* 将文字的左侧定位在父容器的50%位置 */
  transform: translate(-50%, -50%);
  /* 使用transform属性将文字向上和向左移动自身宽高的一半，从而使文字在父容器中垂直和水平居中 */
  color: white;
  font-size: 33px;
  font-weight: bold;
}

.grid-link {
  display: block;
  text-decoration: none;
  color: inherit;
}
</style>
