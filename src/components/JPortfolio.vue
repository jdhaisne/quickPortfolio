<template>
  <div class="portfolio">
    <JElement v-for="elem in portfolioList" :data="elem"></JElement>
  </div>
</template>

<script setup>
import JElement from "./JElement.vue";

const props = defineProps({
  portfolioList: Array,
});
</script>

<style lang="scss" scoped>
.portfolio {
  display: grid;
  gap: 20px;
  grid-template-columns: repeat(auto-fill, 400px);
  justify-content: center;
}
</style>
