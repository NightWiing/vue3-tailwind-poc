<template>
  <input
    type="checkbox"
    v-model="modelValue"
    class="border-gray-300 rounded h-4 w-4"
  />
</template>

<script setup lang="ts">
const modelValue = defineModel()
</script>
