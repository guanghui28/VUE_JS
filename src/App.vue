<!-- eslint-disable no-unused-vars -->
<script setup>
import { ref, reactive, computed, onMounted, onBeforeMount } from 'vue'

onMounted(() => {
  console.log('Component Mounted')
})

onBeforeMount(() => {
  console.log('Before mounted')
})
</script>

<template>
  <h1>Hello world</h1>
</template>

<style></style>
