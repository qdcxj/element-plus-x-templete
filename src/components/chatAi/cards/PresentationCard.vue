<template>
  <el-card class="feature-card presentation-card">
    <div class="card-header">
      <h3>PPT制作</h3>
      <p>图文并茂，自动智能生成PPT</p>
    </div>
    <div class="presentation-content">
      <div class="presentation-icon">
        <el-icon><PictureFilled /></el-icon>
      </div>
      <div class="presentation-text">
        <p>图文并茂，自动智能生成PPT</p>
      </div>
    </div>
  </el-card>
</template>

<script setup>
import { PictureFilled } from '@element-plus/icons-vue'
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

.presentation-content {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background-color: var(--card-bg);
  border-radius: 8px;
  cursor: pointer;
}

.presentation-content:hover {
  background-color: var(--hover-bg);
}

.presentation-icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background-color: #fb923c;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}

.presentation-icon .el-icon {
  font-size: 24px;
}

.presentation-text {
  flex: 1;
}

.presentation-text p {
  font-size: 14px;
  color: var(--text-secondary);
}
</style>