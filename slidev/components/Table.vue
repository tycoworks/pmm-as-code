<script setup>
defineProps({
  xAxisLabel: { type: String, required: true },
  yAxisLabel: { type: String, required: true },
  columnHeaders: { type: Array, required: true },
  rowHeaders: { type: Array, required: true },
  cells: { type: Array, required: true }
})
</script>

<template>
  <div
    class="grid gap-1 items-stretch"
    :style="{ gridTemplateColumns: `auto auto repeat(${columnHeaders.length}, 1fr)` }"
  >
    <!-- Row 1: X axis label spanning data columns -->
    <div></div>
    <div></div>
    <div
      :style="{ gridColumn: `span ${columnHeaders.length}` }"
      class="text-center mb-1 text-xs opacity-70"
    >
      {{ xAxisLabel }}
    </div>

    <!-- Row 2: Column headers -->
    <div></div>
    <div></div>
    <div
      v-for="header in columnHeaders"
      :key="header"
      class="p-2 text-center text-xs font-medium"
    >
      {{ header }}
    </div>

    <!-- Data rows with Y axis label spanning them -->
    <div
      :style="{ gridRow: `span ${rowHeaders.length}` }"
      class="w-6 flex items-center justify-center text-xs opacity-70"
    >
      <span style="writing-mode: vertical-rl; transform: rotate(180deg);">
        {{ yAxisLabel }}
      </span>
    </div>

    <!-- First data row -->
    <div class="p-2 flex items-center text-xs font-medium">
      {{ rowHeaders[0] }}
    </div>
    <div
      v-for="(cell, colIndex) in cells[0]"
      :key="`0-${colIndex}`"
      :class="['grid-cell', `grid-cell-${cell.color || 'high'}`]"
    >
      {{ cell.text || '' }}
    </div>

    <!-- Remaining data rows -->
    <template v-for="(row, rowIndex) in rowHeaders.slice(1)" :key="row">
      <div class="p-2 flex items-center text-xs font-medium">
        {{ row }}
      </div>
      <div
        v-for="(cell, colIndex) in cells[rowIndex + 1]"
        :key="`${rowIndex + 1}-${colIndex}`"
        :class="['grid-cell', `grid-cell-${cell.color || 'high'}`]"
      >
        {{ cell.text || '' }}
      </div>
    </template>
  </div>
</template>
