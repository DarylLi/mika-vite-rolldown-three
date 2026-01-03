<script setup lang="ts">
import { startRender } from './utils.js';
import { onMounted } from 'vue';
onMounted(() => {
  startRender();
});
</script>
<template>
  <div id="container">
    <slot name="default" />
  </div>
</template>
<style scoped>
#container {
  position: absolute;
  z-index: 1;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
