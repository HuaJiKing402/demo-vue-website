<script setup lang="ts">
import BasicLayout from "./layouts/BasicLayout.vue";
import SkinCard from "./components/SkinCard.vue";
</script>
<template>
  <BasicLayout>
    <a-layout-content :style="{ padding: '0 50px', marginTop: '64px' }">
      <a-flex wrap="wrap" gap="small">
        <SkinCard v-for="item in new Array(24)" :key="item" type="primary">Button</SkinCard>
      </a-flex>
    </a-layout-content>
  </BasicLayout>
</template>