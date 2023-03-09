<template>
  <div class="header">
    <div class="header__title">{{ title }}</div>
    <div class="header__slogan">{{ slogan }}</div>
    <div class="header__features">
      <div class="header__feature-item" v-for="(feature, index) in features" :key="index">
        <div class="header__feature-icon">{{ feature.icon }}</div>
        <div class="header__feature-text">{{ feature.text }}</div>
      </div>
    </div>
  </div>
</template>

<script setup>
const title = 'ChatGPT'
const slogan = '让人工智能更聪明'
const features = [
  { icon: '🚀', text: '快速、准确、智能的智能助手' },
  { icon: '🌐', text: '多语言支持，适应全球用户需求' },
  { icon: '💬', text: '智能聊天，解决人机沟通问题' },
  { icon: '💻', text: '丰富的 API 接口，满足开发需求' }
]
</script>

<style scoped>
.header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 60px;
  padding-bottom: 40px;
  text-align: center;
}

.header__title {
  font-size: 48px;
  font-weight: bold;
  color: #1d3557;
}

.header__slogan {
  margin-top: 20px;
  font-size: 24px;
  font-weight: bold;
  color: #457b9d;
}

.header__features {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 40px;
}

.header__feature-item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-right: 40px;
}

.header__feature-icon {
  font-size: 36px;
}

.header__feature-text {
  margin-top: 10px;
  font-size: 16px;
  color: #6c757d;
}
</style>
