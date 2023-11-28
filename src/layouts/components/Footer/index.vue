<template>
  <footer class="layout-footer">© {{ year }}-火凤品办</footer>
</template>

<script lang="ts" setup>
const year = new Date().getFullYear()
</script>
<style lang="scss" scoped>
.layout-footer {
  width: 100%;
  min-height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #c0c4cc;
}
</style>
