<template>
  <div class="menu-demo">
    <a-menu mode="horizontal" :default-selected-keys="['/']" @menu-item-click="handleMenuItemClick">
      <a-menu-item key="/">上传文件</a-menu-item>
      <a-menu-item key="/history">历史记录</a-menu-item>
      <a-menu-item key="/setting">设置</a-menu-item>
    </a-menu>
  </div>
  <RouterView />
</template>
<script setup>
// 引入路由
import { useRouter } from 'vue-router'
const router = useRouter()

// 监听菜单变化，然后改变路由
function handleMenuItemClick(key) {
  router.push({ path: key })
}
</script>
<style scoped lang="scss"></style>
