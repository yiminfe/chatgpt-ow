<template>
  <nav class="navbar">
    <div class="navbar__logo">
      <a href="/">
        <span class="logo">π€</span>
        <span class="title">{{ title }}</span>
      </a>
    </div>
    <ul class="navbar__links">
      <li>
        <a href="#about">
          <span class="icon">π</span>
          <span class="link-text">{{ about }}</span>
        </a>
      </li>
      <li>
        <a href="#features">
          <span class="icon">π</span>
          <span class="link-text">{{ features }}</span>
        </a>
      </li>
      <li>
        <a href="#services">
          <span class="icon">πΌ</span>
          <span class="link-text">{{ services }}</span>
        </a>
      </li>
      <li>
        <a href="#contact">
          <span class="icon">π§</span>
          <span class="link-text">{{ contact }}</span>
        </a>
      </li>
    </ul>
  </nav>
</template>

<script setup>
const title = 'ChatGPT'
const about = 'ε³δΊζδ»¬'
const features = 'δΈ»θ¦εθ½'
const services = 'ζε‘'
const contact = 'θη³»ζδ»¬'
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px;
  background-color: #f8f8f8;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
}

.navbar__logo {
  display: flex;
  align-items: center;
  font-size: 24px;
  font-weight: bold;
}

.navbar__logo .logo {
  margin-right: 8px;
}

.navbar__links {
  display: flex;
  align-items: center;
}

.navbar__links li {
  list-style: none;
}

.navbar__links li:not(:last-child) {
  margin-right: 32px;
}

.navbar__links a {
  display: flex;
  align-items: center;
  font-size: 18px;
  color: #4a4a4a;
  text-decoration: none;
}

.navbar__links a:hover {
  color: #2b2b2b;
}

.navbar__links .icon {
  margin-right: 4px;
  font-size: 20px;
}

.navbar__links .link-text {
  font-size: 16px;
}
</style>
