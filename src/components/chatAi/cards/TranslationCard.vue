<template>
  <el-card class="feature-card translation-card">
    <div class="card-header">
      <h3>网页助手</h3>
      <p>AI读取网页，提供解答与分析</p>
    </div>
    <div class="translation-content">
      <div class="translation-icon">
        <el-icon><Connection /></el-icon>
      </div>
      <div class="translation-text">
        <p>AI读取网页，提供解答与分析</p>
      </div>
    </div>
  </el-card>
</template>

<script setup>
import { Connection } from '@element-plus/icons-vue'
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

.translation-content {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 16px;
  background-color: var(--card-bg);
  border-radius: 8px;
  cursor: pointer;
}

.translation-content:hover {
  background-color: var(--hover-bg);
}

.translation-icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background-color: #38bdf8;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}

.translation-icon .el-icon {
  font-size: 24px;
}

.translation-text {
  flex: 1;
}

.translation-text p {
  font-size: 14px;
  color: var(--text-secondary);
}
</style>