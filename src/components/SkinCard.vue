<script setup lang="ts">
import { SettingOutlined, EditOutlined, EllipsisOutlined } from '@ant-design/icons-vue';
</script>

<template>
<a-card class="skin-card" hoverable style="width: 300px">
  <template #cover>
    <a-empty />
  </template>
  <template #actions>
    <setting-outlined key="setting" />
    <edit-outlined key="edit" />
    <ellipsis-outlined key="ellipsis" />
  </template>
</a-card>
</template>

<style scoped>
.skin-card {

}
</style>