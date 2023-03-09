<template>
  <div class="use-cases">
    <h2 class="use-cases-title">ChatGPT 的应用场景和案例</h2>
    <div class="use-cases-list">
      <div class="use-case-item" v-for="useCase in useCases" :key="useCase.id">
        <div class="use-case-item-icon">{{ useCase.icon }}</div>
        <div class="use-case-item-content">
          <h3 class="use-cases-item-title">{{ useCase.title }}</h3>
          <p class="use-cases-item-description">{{ useCase.description }}</p>
          <ul class="use-case-list">
            <li v-for="item in useCase.list" :key="item">{{ item }}</li>
          </ul>
          <a href="#" class="use-cases-item-link">了解更多</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const useCases = [
  {
    id: 1,
    icon: '👥',
    title: '客服机器人',
    description: 'ChatGPT 可以作为在线客服机器人，为用户提供自然的对话体验，解决用户问题。',
    list: [
      '自动回复用户提问，解决常见问题',
      '提供人性化的问候语和交互界面',
      '快速处理客户问题，提高客户满意度'
    ]
  },
  {
    id: 2,
    icon: '📝',
    title: '智能写作助手',
    description: 'ChatGPT 可以作为智能写作助手，提供丰富的内容生成功能，节省写作时间。',
    list: ['自动生成文章段落和标题', '提供多种写作风格和语气', '检查文章的语法和排版']
  },
  {
    id: 3,
    icon: '🎓',
    title: '在线教育',
    description: 'ChatGPT 可以作为在线教育平台的教学助手，为学生提供个性化的学习体验。',
    list: ['为学生提供有针对性的学习计划和内容', '自动批改作业和测试', '提供针对性的反馈和建议']
  },
  {
    id: 4,
    icon: '🚀',
    title: '空间探索',
    description: 'ChatGPT 可以作为航天任务的计划和执行的智能助手，为航天事业的发展提供支持。',
    list: [
      '帮助制定航天任务的计划和执行方案',
      '分析和处理卫星数据和航天器的监测数据',
      '提供实时的数据分析和报告'
    ]
  }
]
</script>

<style scoped>
.use-cases {
  padding: 50px;
}

.use-cases-title {
  margin-top: 0;
  text-align: center;
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
}

.use-cases-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: stretch;
  margin-top: 50px;
}

.use-case-item {
  margin: 20px;
  max-width: 400px;
  width: 100%;
  border: 1px solid #ddd;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  overflow: hidden;
  width: calc(100% - 48px);
  margin-left: 12px;
  transition: all 0.3s ease-in-out;
}

.use-case-item:hover {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  transform: translateY(-5px);
}

.use-case-item-icon {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 64px;
  height: 64px;
  font-size: 2rem;
  color: #fff;
  background-color: #0078ff;
  border-radius: 50%;
  margin-right: 20px;
}

.use-case-item-content {
  padding: 20px;
}

.use-case-item-title {
  margin: 0;
  font-size: 1.5rem;
  font-weight: bold;
  color: #333;
}

.use-case-item-description {
  margin: 10px 0 0;
  font-size: 1rem;
  color: #666;
}

.use-case-item-list {
  margin-top: 10px;
  list-style-type: disc;
  padding-left: 20px;
}

.use-case-item-list li {
  margin-bottom: 5px;
  font-size: 0.9rem;
  color: #666;
}

.use-case-item-link {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  font-size: 1rem;
  font-weight: bold;
  color: #fff;
  background-color: #0078ff;
  border-radius: 5px;
  text-decoration: none;
  transition: all 0.3s ease-in-out;
}

.use-case-item-link:hover {
  background-color: #006ae6;
  transform: translateY(-2px);
}
</style>
