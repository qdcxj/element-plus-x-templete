<template>
  <div class="search-header">
    <div class="search-container">
      <el-button type="primary" class="new-chat-btn">
        <el-icon><Plus /></el-icon>
        新建对话
      </el-button>
      <el-input
        v-model="searchQuery"
        placeholder="搜索"
        class="search-input"
        :prefix-icon="Search"
      />
    </div>
    <div class="history-list">
      <div v-for="(item, index) in historyItems" :key="index" class="history-item">
        {{ item }}
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { Plus, Search } from '@element-plus/icons-vue'

const searchQuery = ref('')
const historyItems = ref([
  '最近7天',
  'TurboFeLv深的作用',
  '通义于文如何生成代码',
  'claude-3.5-sonnet的评测',
  'node-gyp安装成功，node-g',
  '如何将检索到的上下文和用',
  '通义于如何将图像和口述笔'
])
</script>

<style scoped>
.search-header {
  border-bottom: 1px solid var(--border-color);
  border-right: 1px solid var(--border-color);
  padding: 16px;
  background-color: white;
}

.search-container {
  display: flex;
  gap: 10px;
  margin-bottom: 16px;
}

.new-chat-btn {
  display: flex;
  align-items: center;
  gap: 5px;
}

.search-input {
  flex: 1;
}

.history-list {
  overflow-y: auto;
  height: 100%;
}

.history-item {
  padding: 8px 0;
  color: var(--text-secondary);
  font-size: 14px;
  cursor: pointer;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.history-item:hover {
  color: var(--text-primary);
}
</style>