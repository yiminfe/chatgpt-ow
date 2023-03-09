<template>
  <div class="features">
    <h2 class="features-title">ChatGPT 的特点和优势</h2>
    <div class="features-list">
      <div class="features-item">
        <div class="features-item-icon">🚀</div>
        <div class="features-item-content">
          <h3>快速</h3>
          <p>ChatGPT 可以快速地生成高质量的对话，节省您的时间和精力。</p>
        </div>
      </div>
      <div class="features-item">
        <div class="features-item-icon">💬</div>
        <div class="features-item-content">
          <h3>自然</h3>
          <p>ChatGPT 可以生成自然流畅的对话，仿佛在和真人聊天一样。</p>
        </div>
      </div>
      <div class="features-item">
        <div class="features-item-icon">🎨</div>
        <div class="features-item-content">
          <h3>定制</h3>
          <p>ChatGPT 可以根据您的需求进行个性化定制，满足您不同的场景需求。</p>
        </div>
      </div>
      <div class="features-item">
        <div class="features-item-icon">💡</div>
        <div class="features-item-content">
          <h3>创新</h3>
          <p>ChatGPT 使用最新的人工智能技术，不断创新和进步。</p>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.features {
  padding: 50px;
}

.features-title {
  margin-top: 0;
  text-align: center;
  font-size: 2.5rem;
  font-weight: bold;
  color: #333;
}

.features-list {
  margin-top: 50px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 20px;
}

.features-item {
  padding: 30px;
  background-color: #fff;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  display: flex;
  flex-direction: column;
}

.features-item-icon {
  font-size: 3.5rem;
  margin-bottom: 10px;
  color: #6c63ff;
}

.features-item-content {
  flex: 1;
}

.features-item h3 {
  font-size: 1.8rem;
  font-weight: bold;
  color: #333;
  margin-top: 0;
}

.features-item p {
  font-size: 1.4rem;
  color: #666;
}

/* 修改手机端的 features-item 元素的大小 */
@media only screen and (max-width: 768px) {
  .features-item {
    width: 100%;
    padding: 20px;
    margin-bottom: 20px;
  }

  .features-item-icon {
    font-size: 2.5rem;
    margin-right: 20px;
  }

  .features-item h3 {
    font-size: 1.5rem;
  }

  .features-item p {
    font-size: 1.2rem;
  }
}
</style>
