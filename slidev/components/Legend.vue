<script setup lang="ts">
defineProps<{
  items: { label: string; type: string }[]
}>()
</script>

<template>
  <div class="legend">
    <template v-for="(item, index) in items" :key="item.label">
      <span :class="item.type">{{ item.label }}</span>
      <span v-if="index < items.length - 1" class="separator">·</span>
    </template>
  </div>
</template>

<style scoped>
.separator {
  margin: 0 0.75rem;
  color: var(--body-text);
}
</style>
