<template>
  <div class="common-layout">
    <el-container>
      <el-main style="width: 880px;">
        <!-- <div class="common-card">
          <h2 style="margin-bottom: 10px;color: white">镜头语言：</h2>
          <el-input v-model="input" style="width: 240px" placeholder="请输入" />
          <el-button type="primary" style="margin-left: 10px">添加</el-button>
        </div> -->
        
        <el-card style="background-color: grey; margin-bottom: 10px;">
          <template #header>
            <div class="card-header">
              <span>镜头语言</span>
            </div>
          </template>
          <el-checkbox-group v-model="checkboxGroup1" size="small">
            <el-checkbox label="Option1" value="Value1" border />
            <el-checkbox label="Option2" value="Value2" border />
          </el-checkbox-group>
          <template #footer>
            <el-input v-model="input" style="width: 240px" placeholder="请输入" />
            <el-button type="primary" style="margin-left: 10px">添加</el-button>
          </template>
        </el-card>

        <el-card style="max-width: 480px; background-color: grey;">
          <template #header>
            <div class="card-header">
              <span>镜头语言：</span>
            </div>
          </template>
          <el-input v-model="input" style="width: 240px" placeholder="请输入" />
          <el-button type="primary" style="margin-left: 10px">添加</el-button>
          <template #footer>Footer content</template>
        </el-card>

      </el-main>
    </el-container>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const input = ref('')
const checkboxGroup1 = ref(['Value1'])
</script>

<style>
body{
  background-color: #000;
}
#app {
  color: aqua;
  margin-left: 0;
}
.common-card{
  background-color: grey;
  display: flex;
}
</style>
