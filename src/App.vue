<template>
  <div>
    <h1>{{ title }}</h1>
    <p>計數器: {{ counter }}</p>
    <button @click="incrementCounter">增加</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const title = ref('Vue 3 簡單範例')
const counter = ref(0)

function incrementCounter() {
  counter.value++
}
</script>

<style scoped>
/* 您可以在這裡添加任何組件特定的樣式 */
</style>