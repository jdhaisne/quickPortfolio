<template>
  <div class="elem">
    <h2 class="elem__title">{{ props.data.title }}</h2>
    <img width="394.5" height="264" class="elem__img" :src="props.data.img" />
    <div class="elem__desc">{{ props.data.desc }}</div>
    <div class="elem__link__wrapper">
      <a class="elem__link elem__link--vercel" :href="props.data.vercelLink"
        >Live version</a
      >
      <a class="elem__link elem__link--git" :href="props.data.gitLink"
        >github</a
      >
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  data: Object, // vercelLink, gitLink, desc, img, title,
});
</script>

<style lang="scss" scoped>
.elem {
  display: flex;
  flex-direction: column;
  place-items: center;
  &__title {
  }
  &__img {
  }
  &__desc {
  }
  &__link {
    &__wrapper {
      display: flex;
      justify-content: space-between;
      width: 100%;
    }
  }
}
</style>
