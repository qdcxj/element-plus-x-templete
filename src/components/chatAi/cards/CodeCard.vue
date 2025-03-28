<template>
  <el-card class="feature-card code-card">
    <div class="card-header">
      <h3>代码格式</h3>
      <p>代码格式化与优化</p>
    </div>
    <div class="code-preview">
      <div class="code-window">
        <div class="window-header">
          <div class="window-dots">
            <span class="dot red"></span>
            <span class="dot yellow"></span>
            <span class="dot green"></span>
          </div>
          <div class="window-title">Hello.js</div>
        </div>
        <div class="code-content">
          <pre><code>let name = "world";
function hello() {
  return "Hello, " + 
    name + "!";
}</code></pre>
        </div>
      </div>
      <div class="code-label">代码优化模式</div>
    </div>
  </el-card>
</template>

<script setup>
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

.code-preview {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.code-window {
  border-radius: 8px;
  overflow: hidden;
  border: 1px solid var(--border-color);
}

.window-header {
  background-color: #f3f4f6;
  padding: 8px 12px;
  display: flex;
  align-items: center;
}

.window-dots {
  display: flex;
  gap: 6px;
  margin-right: 12px;
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
}

.dot.red {
  background-color: #ef4444;
}

.dot.yellow {
  background-color: #f59e0b;
}

.dot.green {
  background-color: #10b981;
}

.window-title {
  font-size: 12px;
  color: var(--text-secondary);
}

.code-content {
  padding: 12px;
  background-color: white;
  font-family: 'Menlo', 'Monaco', 'Courier New', monospace;
  font-size: 12px;
  line-height: 1.5;
  color: #374151;
  overflow-x: auto;
}

.code-label {
  font-size: 12px;
  color: var(--text-secondary);
  text-align: center;
}
</style>