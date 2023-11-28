<template>
  <div class="flex justify-center items-center">
    {{ counter }}
  </div>
</template>

<script setup lang="ts">
import { useIntervalFn } from "@vueuse/core"
import { ref } from "vue"
const counter = ref(0)
const { resume } = useIntervalFn(() => {
  counter.value++
}, 1000)
resume()
</script>

<style scoped></style>
