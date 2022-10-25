<script setup>
import AtomSpanVue from "../Atoms/AtomSpan.vue";

defineProps({
  list: Array,
});
</script>

<template>
  <ul class="items">
    <li v-for="(info, index) in list" :key="index">
      <AtomSpanVue :class="'item'">{{ info }}</AtomSpanVue>
    </li>
  </ul>
</template>
