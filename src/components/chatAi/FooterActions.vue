<template>
  <div class="footer-actions">
    <div class="action-buttons">
      <el-button type="text" class="action-btn">
        <el-icon><Document /></el-icon>
        文章思考
      </el-button>
      <el-button type="text" class="action-btn">
        <el-icon><RefreshRight /></el-icon>
        知识搜索
      </el-button>
      <el-button type="text" class="action-btn">
        <el-icon><Brush /></el-icon>
        代码模式
      </el-button>
      <el-button type="text" class="action-btn">
        <el-icon><PictureFilled /></el-icon>
        PPT制作
      </el-button>
      <el-button type="text" class="action-btn">
        <el-icon><Setting /></el-icon>
        设置中心
      </el-button>
    </div>
    <Sender>
      <!-- 自定义操作列表 -->
      <template #action-list>
        <div class="action-list-self-wrap">
          <el-button type="danger" circle>
            <el-icon><Delete /></el-icon>
          </el-button>

          <el-button type="primary" circle style="rotate: -45deg;">
            <el-icon><Position /></el-icon>
          </el-button>
        </div>
      </template>
    </Sender>
  </div>
</template>

<script setup>
import { Document, RefreshRight, Brush, PictureFilled, Setting, Upload, Position,Delete } from '@element-plus/icons-vue'
</script>

<style scoped>
.footer-actions {
  border-top: 1px solid var(--border-color);
  padding: 12px 10%;
  background-color: white;
}

.action-buttons {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin-bottom: 16px;
  flex-wrap: wrap;
}

.action-btn {
  display: flex;
  align-items: center;
  gap: 4px;
  color: var(--text-secondary);
  font-size: 14px;
}

.action-btn:hover {
  color: var(--primary-color);
}

.input-area {
  display: flex;
  align-items: center;
  border: 1px solid var(--border-color);
  border-radius: 24px;
  padding: 8px 16px;
  background-color: white;
}

.upload-btn, .send-btn {
  color: var(--text-secondary);
}

.upload-btn:hover, .send-btn:hover {
  color: var(--primary-color);
}

.input-placeholder {
  flex: 1;
  color: var(--text-secondary);
  font-size: 14px;
  text-align: center;
}
.action-list-self-wrap{
  width: 80px;
}
</style>