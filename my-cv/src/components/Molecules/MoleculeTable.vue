<script setup>
defineProps({
  data: Object,
});
</script>

<template>
  <table class="table table-sm table-borderless table-responsive">
    <tbody>
      <tr v-for="(info, index) in data" :key="index">
        <td class="p-1 pr-2 font-weight-bold">
          <b>{{ info.label }}</b>
        </td>
        <td class="p-1 pl-2 font-weight-light text">
          {{ info.value }}
        </td>
      </tr>
    </tbody>
  </table>
</template>
