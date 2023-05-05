<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import JPortfolio from "./components/JPortfolio.vue";
</script>

<template>
  <h1>jdhaisne's project</h1>
  <JPortfolio
    :portfolio-list="[
      {
        title: 'kanban',
        img: '/src/assets/imgs/kanbanScreen.png',
        desc: 'A Simple kanban demonstration from front end mentor',
        vercelLink: 'https://kanban-task-management-five.vercel.app/',
        gitLink: 'https://github.com/jdhaisne/kanban-task-management',
      },
      {
        title: 'fylo data storage',
        img: '/src/assets/imgs/fyloScreen.png',
        desc: 'A Simple animation from front end mentor',
        vercelLink: 'https://fylo-data-storage-component-inky-beta.vercel.app/',
        gitLink: 'https://github.com/jdhaisne/fylo-data-storage-component',
      },
      {
        title: 'social proof section',
        img: '/src/assets/imgs/socialScreen.png',
        desc: 'A Simple example of social proof from front end mentor',
        vercelLink: 'https://social-proof-section-master-lilac.vercel.app',
        gitLink: 'https://github.com/jdhaisne/social-proof-section-master',
      },
      {
        title: 'profil card',
        img: '/src/assets/cardScreen.png',
        desc: 'A Simple profil card from front end mentor',
        vercelLink: 'https://profile-card-component-j5fwc0nuv.vercel.app/',
        gitLink: 'https://github.com/jdhaisne/profile-card-component',
      },
    ]"
  ></JPortfolio>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
