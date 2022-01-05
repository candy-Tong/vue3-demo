<template>
  <AddOne :count='count' @add='add' />
</template>
<script setup lang='ts'>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import AddOne from './components/AddOne.vue'
import { ref } from 'vue'

const count = ref(0)

function add() {
  count.value = count.value + 1
}
</script>


