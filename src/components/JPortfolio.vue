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
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
