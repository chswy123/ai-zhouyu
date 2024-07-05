<template>
  <div class="left-align-container">
    <h2 style="margin-bottom: 10px;color: white">镜头语言：</h2>
    <el-input v-model="input" style="width: 240px" placeholder="请输入" />
    <el-button type="primary" style="margin-left: 10px">添加</el-button>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const input = ref('')
</script>

<style scoped>
:global(body) {
  background-color: black;
}
.left-align-container {
  text-align: left;
}
</style>
