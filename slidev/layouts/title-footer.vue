<script setup>
import { computed } from 'vue'

const props = defineProps({
  cols: {
    type: Number,
    default: 1
  }
})

const gridClass = computed(() => {
  if (props.cols === 2) return 'grid-cols-2'
  if (props.cols === 3) return 'grid-cols-3'
  return ''
})
</script>

<template>
  <div class="slidev-layout title-footer">
    <div class="header">
      <slot name="title" />
    </div>
    <div class="content">
      <template v-if="cols === 1">
        <slot />
      </template>
      <div v-else :class="`grid ${gridClass} gap-6 items-stretch h-full`">
        <div class="flex flex-col"><slot name="col1" /></div>
        <div class="flex flex-col"><slot name="col2" /></div>
        <div v-if="cols >= 3" class="flex flex-col"><slot name="col3" /></div>
      </div>
    </div>
    <div class="footer">
      <slot name="footer" />
    </div>
  </div>
</template>

<style scoped>
.title-footer {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.header {
  flex-shrink: 0;
}

.content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.footer {
  flex-shrink: 0;
}
</style>
