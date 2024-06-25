<script setup>
import { ref, reactive, computed } from 'vue'

const numbers = ref([1, 2, 3, 4, 5])
const evenNumbers = computed(() => {
  return numbers.value.filter((n) => n % 2 === 0)
})
</script>

<template>
  <ul>
    <li v-for="n in evenNumbers" :key="n">
      {{ n }}
    </li>
  </ul>
</template>

<style>
.button {
  border: none;
  color: #8b5cf6;
  background: #ede9fe;
  padding: 10px 14px;
  border-radius: 6px;
  cursor: pointer;

  &:hover {
    background-color: #c7d2fe;
  }
}

.active {
  background: #8b5cf6;
  color: #ede9fe;

  &:hover {
    background-color: #818cf8;
  }
}

.has-error {
  background: #ef4444;
  color: #fee2e2;

  &:hover {
    background-color: #ef2266;
  }
}
</style>
