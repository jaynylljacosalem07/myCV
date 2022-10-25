<script setup>
import AtomH3Vue from "../Atoms/AtomH3.vue";
import MoleculeTable from "../Molecules/MoleculeTable.vue";
import MoleculeList from "../Molecules/MoleculeList.vue";

defineProps({
  card_title: String,
  table_list: Object,
  list: Array,
  data: Object,
});
</script>
<template>
  <div class="card mt-3 p-3">
    <AtomH3Vue :text="data.title"></AtomH3Vue>
    <div>
      <template v-if="data.table">
        <MoleculeTable :data="data.table"></MoleculeTable>
      </template>
      <template v-if="data.list">
        <MoleculeList :list="data.list"></MoleculeList>
      </template>
    </div>
  </div>
</template>
