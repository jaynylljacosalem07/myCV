<script setup>
import { reactive } from "vue";
import OraganismCardVue from "./components/Organisms/OraganismCard.vue";

const cards = reactive([
  {
    title: "General Information",
    table: [
      { label: "Full Name", value: "Jaynyll Justiniani Jacosalem" },
      { label: "Date of Birth", value: " 7th September 1991" },
      { label: "Languages", value: "English, Tagalog, Visayan" },
    ],
  },
  {
    title: "Education",
    list: ["BACHELOR OF SCIENCE IN INFORMATION TECHNOLOGY"],
  },
]);
</script>

<template>
  <OraganismCardVue
    v-for="(card, index) in cards"
    :key="index"
    :data="card"
  ></OraganismCardVue>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
