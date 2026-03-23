<script setup lang="ts">
import { onMounted, ref } from 'vue';

const config = useRuntimeConfig();
const apiBase = config.public.apiBase;

const initData = ref([]);

onMounted(() => {
  initData.value = 'Hello world';
});

</script>
<template>
  <div>
    {{ initData }}
  </div>
</template>
<style scoped>
</style>