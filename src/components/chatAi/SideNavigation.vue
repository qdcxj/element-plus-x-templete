<template>
  <div class="side-navigation">
    <div class="logo">
      <el-icon><Setting /></el-icon>
      <span>通义</span>
    </div>
    
    <div class="nav-items">
      <div class="nav-item active">
        <el-icon><ChatDotRound /></el-icon>
        <span>对话</span>
      </div>
      <div class="nav-item">
        <el-icon><Promotion /></el-icon>
        <span>发现</span>
      </div>
      <div class="nav-item">
        <el-icon><User /></el-icon>
        <span>我的助手</span>
      </div>
      <div class="nav-item">
        <el-icon><Folder /></el-icon>
        <span>笔记库</span>
      </div>
    </div>
    
    <div class="bottom-actions">
      <div class="nav-item">
        <el-icon><Document /></el-icon>
      </div>
      <div class="nav-item">
        <!-- <el-icon><Mobile /></el-icon> -->
      </div>
      <div class="nav-item">
        <el-icon><Avatar /></el-icon>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Setting, ChatDotRound, Promotion, User, Folder, Document, Avatar } from '@element-plus/icons-vue'
</script>

<style scoped>
.side-navigation {
  width: 60px;
  background-color: var(--sidebar-bg);
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 16px 0;
  height: 100%;
}

.logo {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 30px;
  font-size: 12px;
}

.logo .el-icon {
  font-size: 24px;
  margin-bottom: 4px;
}

.nav-items {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 30px;
  flex: 1;
}

.nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  cursor: pointer;
  font-size: 12px;
  opacity: 0.8;
  transition: opacity 0.2s;
}

.nav-item:hover, .nav-item.active {
  opacity: 1;
}

.nav-item .el-icon {
  font-size: 20px;
  margin-bottom: 4px;
}

.bottom-actions {
  margin-top: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}
</style>