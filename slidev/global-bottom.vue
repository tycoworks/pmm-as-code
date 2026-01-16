<script setup>
import { useSlideContext } from '@slidev/client'

const { $page, $nav } = useSlideContext()
</script>

<template>
  <div class="page-number">
    {{ $page }} / {{ $nav.total }}
  </div>
</template>

<style scoped>
.page-number {
  position: fixed;
  bottom: 1rem;
  right: 1.5rem;
  font-size: 0.75rem;
  color: var(--gray-text);
  z-index: 100;
}
</style>
