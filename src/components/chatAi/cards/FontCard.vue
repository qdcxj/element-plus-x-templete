<template>
  <el-card class="feature-card font-card">
    <div class="card-header">
      <h3>精选智能体</h3>
      <p>Qwen-QwQ 3.5B</p>
    </div>
    <div class="font-content">
      <div class="font-icon">
        <!-- <el-icon><Magic /></el-icon> -->
      </div>
      <div class="font-text">
        <p>轻快轻量级模型可以下载使用</p>
      </div>
    </div>
  </el-card>
</template>

<script setup>
// import { Magic } from '@element-plus/icons-vue'
</script>

<style scoped>
.feature-card {
  flex: 1;
  min-width: 300px;
  height: 100%;
}

.card-header {
  margin-bottom: 16px;
}

.card-header h3 {
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 4px;
  color: var(--text-primary);
}

.card-header p {
  font-size: 12px;
  color: var(--text-secondary);
}

.font-content {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background-color: var(--card-bg);
  border-radius: 8px;
  cursor: pointer;
}

.font-content:hover {
  background-color: var(--hover-bg);
}

.font-icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background-color: #a78bfa;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}

.font-icon .el-icon {
  font-size: 24px;
}

.font-text {
  flex: 1;
}

.font-text p {
  font-size: 14px;
  color: var(--text-secondary);
}
</style>