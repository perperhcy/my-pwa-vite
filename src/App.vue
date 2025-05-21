<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <a href="https://vite.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const isStandalone = window.matchMedia('(display-mode: standalone)').matches
  const launchMode = isStandalone ? 'PWA 模式' : '浏览器模式'
  document.getElementById('launch-mode').textContent = `当前打开方式：${launchMode}`
})
</script>

<template>
  <!-- 您的其他模板内容 -->
</template>

<style scoped>
#launch-mode {
  position: fixed;
  bottom: 20px;
  right: 20px;
  padding: 10px;
  background-color: #f0f0f0;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
</style>
