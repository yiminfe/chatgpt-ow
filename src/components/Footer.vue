<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__section">
        <h4>{{ companyName }}</h4>
        <p>{{ companyDesc }}</p>
        <ul>
          <li><a href="#">关于我们</a></li>
          <li><a href="#">团队介绍</a></li>
          <li><a href="#">加入我们</a></li>
        </ul>
      </div>
      <div class="footer__section">
        <h4>联系我们</h4>
        <p>{{ contactInfo }}</p>
        <ul>
          <li><a href="#">联系电话</a></li>
          <li><a href="#">电子邮件</a></li>
          <li><a href="#">地址</a></li>
        </ul>
      </div>
      <div class="footer__section">
        <h4>版权声明</h4>
        <p>{{ copyright }}</p>
        <ul>
          <li><a href="#">隐私政策</a></li>
          <li><a href="#">使用条款</a></li>
        </ul>
      </div>
    </div>
    <div class="footer__text">
      <hr />
      <p>{{ footerText }}</p>
    </div>
  </footer>
</template>

<script setup>
const companyName = 'ChatGPT'
const companyDesc = '我们是一家致力于提供高品质聊天机器人技术的公司'
const contactInfo =
  '联系电话：400-888-8888\n电子邮件：contact@chatgpt.com\n地址：北京市海淀区XX街XX号'
const footerText = `© ${new Date().getFullYear()} ${companyName}. All Rights Reserved.`
const copyright =
  '本网站所刊载信息，如无特别说明，均为ChatGPT的原创。未经授权禁止复制或建立镜像，违者依法将被追究法律责任。'
</script>

<style scoped>
.footer {
  background-color: #f8f9fa;
  padding: 30px 0;
}

.footer .container {
  display: flex;
  justify-content: center;
}

.footer__section {
  display: inline-block;
  width: 25%;
  padding: 0px 20px;
  vertical-align: top;
}

.footer__section h4 {
  font-size: 20px;
  margin-bottom: 20px;
}

.footer__section ul {
  padding-left: 0;
  list-style: none;
  margin-bottom: 40px;
}

.footer__section li {
  margin-bottom: 10px;
}

.footer__section a {
  color: #6c757d;
  text-decoration: none;
}

.footer__text {
  text-align: center;
  margin-top: 40px;
  border-top: 1px solid #6c757d;
}

.footer__text hr {
  margin: 0 auto;
  width: 50%;
  border-top: none;
  border-bottom: 1px solid #6c757d;
}

.footer__text p {
  margin-top: 20px;
  font-size: 14px;
  color: #6c757d;
}
</style>
