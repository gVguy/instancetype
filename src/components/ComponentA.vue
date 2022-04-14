<template>
  <h1>{{ text }}</h1>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const text = ref('hello')

function setText(data: string) {
  text.value = data
}

defineExpose({ setText })
</script>
