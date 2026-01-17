<script setup>
defineProps({
  items: {
    type: Array,
    required: true
  },
  columns: {
    type: Number,
    default: 3
  }
})
</script>

<template>
  <div
    class="grid"
    :style="{ gridTemplateColumns: `repeat(${columns}, 1fr)` }"
  >
    <div v-for="(item, index) in items" :key="index" class="grid-item">
      <div class="item-number">{{ String(index + 1).padStart(2, '0') }}</div>
      <h3 class="item-title">{{ item.title }}</h3>
      <div class="item-description">{{ item.description }}</div>
    </div>
  </div>
</template>

<style scoped>
.grid {
  display: grid;
  gap: 1.5rem 2rem;
}

.grid-item {
  display: flex;
  flex-direction: column;
}

.item-number {
  color: var(--gray-text);
  font-size: 0.9rem;
  padding-bottom: 0.3rem;
  border-bottom: 0.5px solid currentColor;
  margin-bottom: 0.5rem;
}

.item-title {
  font-size: 1.1rem;
  margin: 0 0 0.3rem 0;
}

.item-description {
  font-size: 0.85rem;
  color: var(--body-text);
  line-height: 1.4;
}
</style>
