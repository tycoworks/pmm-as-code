<script setup>
defineProps({
  type: {
    type: String,
    default: 'info',
  },
  title: {
    type: String,
    default: '',
  },
})
</script>

<template>
  <div :class="['admonition', `admonition-${type}`]" class="flex-1">
    <div v-if="title" class="admonition-title">
      {{ title }}
    </div>
    <div class="admonition-content">
      <slot />
    </div>
  </div>
</template>
