<template>
  <el-card class="feature-card tools-card">
    <div class="card-header">
      <h3>效率工具</h3>
      <p>为各类场景提供高效工具</p>
    </div>
    <div class="tools-grid">
      <div class="tool-item">
        <div class="tool-icon blue">
          <el-icon><Document /></el-icon>
        </div>
        <div class="tool-info">
          <div class="tool-name">实时记录</div>
          <div class="tool-desc">语音转文字，为场景提供解决方案</div>
        </div>
      </div>
      <div class="tool-item">
        <div class="tool-icon green">
          <el-icon><ChatLineRound /></el-icon>
        </div>
        <div class="tool-info">
          <div class="tool-name">网页助手</div>
          <div class="tool-desc">AI读取网页，提供解答与分析</div>
        </div>
      </div>
    </div>
  </el-card>
</template>

<script setup>
import { Document, ChatLineRound } from '@element-plus/icons-vue'
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

.tools-grid {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.tool-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px;
  border-radius: 8px;
  cursor: pointer;
}

.tool-item:hover {
  background-color: var(--hover-bg);
}

.tool-icon {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
}

.tool-icon.blue {
  background-color: #60a5fa;
}

.tool-icon.green {
  background-color: #34d399;
}

.tool-icon .el-icon {
  font-size: 20px;
}

.tool-info {
  flex: 1;
}

.tool-name {
  font-size: 14px;
  font-weight: 500;
  margin-bottom: 2px;
  color: var(--text-primary);
}

.tool-desc {
  font-size: 12px;
  color: var(--text-secondary);
}
</style>