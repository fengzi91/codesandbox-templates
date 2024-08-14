<script setup>
import { ref } from 'vue'
import { ElButton } from 'element-plus'
import { ElInput } from 'element-plus'

const message = ref('')
</script>
<template>
  <div class="page">
    <div class="container">
      <div>
        <ElButton type="primary">主要按钮</ElButton>
        <ElButton type="success">成功按钮</ElButton>
        <ElButton type="warning">警告按钮</ElButton>
        <ElButton type="danger">危险按钮</ElButton>
      </div>
      <ElInput v-model="message" placeholder="请输入内容"></ElInput>
      <div class="message">
        <span style="font-size: 12px">输入的内容是：</span>
        <span>{{ message }}</span>
      </div>
      <el-button @click="message = ''">重置</el-button>
    </div>
  </div>
</template>
<style scoped>
.page {
  min-height: 100vh;
  width: 100vw;
  max-width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #f0f2f5;
}
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  row-gap: 20px;
}
.message {
  display: grid;
  grid-template-columns: 140px 1fr;
  width: 100%;
}
</style>
