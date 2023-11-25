<template>
  <div class="flex justify-center">
    {{ counter }}
  </div>
</template>

<script setup lang="ts">
import { useInterval } from "@vueuse/core"
const { resume, counter } = useInterval(1000, { controls: true })
resume()
</script>

<style scoped></style>
