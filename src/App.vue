<script setup>
import { RouterLink, RouterView } from "vue-router";
import TheHeader from "./components/sections/TheHeader.vue";
import TheFooter from "./components/sections/TheFooter.vue";
</script>

<template>
  <div id="layout">
    <TheHeader />

    <main>
      <RouterView />
    </main>

    <TheFooter />
  </div>
</template>

<style scoped>
#layout {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr max-content;
  min-height: 100vh;
}
</style>
