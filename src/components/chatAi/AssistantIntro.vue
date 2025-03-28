<template>
  <div class="assistant-intro">
    <div class="avatar">
      <img src="https://hebbkx1anhila5yf.public.blob.vercel-storage.com/screenshot-20250328-100913-tzSTURnLGfD0HIXxTk0sUwlgUmSMfh.png" alt="通义 AI 助手" class="avatar-img" />
    </div>
    <div class="intro-text">
      <h2>我是通义，你的个人AI助手</h2>
      <p>我可以帮你处理各类事情，<el-link type="primary">这一版 <el-icon class="el-icon--right"><ArrowRight /></el-icon></el-link></p>
    </div>
  </div>
</template>

<script setup>
import { ArrowRight } from '@element-plus/icons-vue'
</script>

<style scoped>
.assistant-intro {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-top: 40px;
  margin-bottom: 20px;
  width: 100%;
  max-width: 800px;
}

.avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  overflow: hidden;
  background-color: var(--primary-color);
  display: flex;
  align-items: center;
  justify-content: center;
}

.avatar-img {
  width: 40px;
  height: 40px;
  object-fit: contain;
}

.intro-text h2 {
  font-size: 20px;
  font-weight: 600;
  margin-bottom: 8px;
  color: var(--text-primary);
}

.intro-text p {
  font-size: 14px;
  color: var(--text-secondary);
}
</style>