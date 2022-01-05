<template>
  <h1>{{ count }}</h1>
  <button @click="emit('add')">AddOne</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
defineProps<{ count: number }>()
const emit = defineEmits(['add'])
</script>
