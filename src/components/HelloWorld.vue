<template>
  <ComponentA ref="a" />
</template>

<script setup lang="ts">
import { ref } from 'vue'

import ComponentA from './ComponentA.vue'

const a = ref<InstanceType <typeof ComponentA>>()

setTimeout(() => a.value.setText(22), 1000)
</script>
