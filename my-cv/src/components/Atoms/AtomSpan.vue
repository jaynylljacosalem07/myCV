<script setup>
defineProps({
  text: String,
  class: String,
});
</script>

<template>
  <span
    class="class.length > 0 ? class : 'badge font-weight-bold danger-color-dark text-uppercase align-middle min-width'"
    >{{ text }}</span
  >
</template>

<style scoped>
.min-width {
  min-width: 75px;
}
</style>
