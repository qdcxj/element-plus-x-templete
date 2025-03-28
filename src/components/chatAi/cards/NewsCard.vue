<template>
  <el-card class="feature-card news-card">
    <div class="card-header">
      <h3>今日热度</h3>
      <p>全球最新热点话题整理</p>
    </div>
    <div class="news-list">
      <div v-for="(item, index) in newsItems" :key="index" class="news-item">
        <span class="news-index">{{ index + 1 }}</span>
        <span class="news-title">{{ item }}</span>
      </div>
    </div>
  </el-card>
</template>

<script setup>
import { ref } from 'vue'

const newsItems = ref([
  '3月27日，深度交通检查部署展...',
  '银行春招招聘即将，科技岗位...',
  '国际机构预计中国经济，预测...',
  '知乎青少年使用与分享，AI比...',
  '预计2025年柳市市场规模，稳...'
])
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

.news-list {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.news-item {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 14px;
  cursor: pointer;
}

.news-index {
  color: var(--primary-color);
  font-weight: 600;
}

.news-title {
  color: var(--text-secondary);
  flex: 1;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.news-item:hover .news-title {
  color: var(--text-primary);
}
</style>