<script setup lang="ts">
import { UserOutlined } from '@ant-design/icons-vue';
</script>

<template>
  <a-layout>
    <a-layout-header>
      <a-flex justify="around" align="center">
        <div class="logo"/>
        <a-menu
            v-model:selectedKeys="selectedKeys"
            theme="dark"
            mode="horizontal"
            :style="{ lineHeight: '64px' }">
          <a-menu-item key="1">首页</a-menu-item>
          <a-menu-item key="2">nav 2</a-menu-item>
          <a-menu-item key="3">nav 3</a-menu-item>
        </a-menu>
        <a-space style="text-overline-color: red">
          <a-avatar shape="square" :size="40" style="color: #f56a00; background-color: #fde3cf">
            <template #icon><UserOutlined /></template>
          </a-avatar>
          HuaJiKing402
        </a-space>

      </a-flex>
    </a-layout-header>

    <a-layout-content>
      <slot class="content"/>
    </a-layout-content>

    <a-layout-footer :style="{ textAlign: 'center' }">
      Ant Design ©2018 Created by Ant UED
    </a-layout-footer>
  </a-layout>
</template>

<style scoped>
.logo {
  width: 120px;
  height: 31px;
  background: rgba(255, 255, 255, 0.2);
  margin: 16px 24px 16px 0;
  float: left;
}
.site-layout .site-layout-background {
  background: #fff;
}

[data-theme='dark'] .site-layout .site-layout-background {
  background: #141414;
}
</style>