<script setup>
import { useRoute } from "vue-router";
import { computed } from "vue";
const route = useRoute();

const header_home = computed(() => {
  return route.path == "/" ? "header_home" : "";
});
</script>

<template>
  <header :class="header_home">
    <div>
      <h1>About me</h1>
    </div>
    <div>
      <img class="logo_header" src="/images/logo.svg" alt="Logo" />
    </div>
    <h1>My projects</h1>
    <!-- <div>
        <a href="">Branding & Packaging</a>
        <a href="">Illustrations & Prints</a>
        <a href="">Photographs & Audiovisual Content</a>
        <a href="">3D Modelling & Animations</a>
      </div> -->
  </header>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Italiana&display=swap");

header {
  height: 120px;
  color: var(--color-white);
  background-color: var(--primary-first);
  width: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  justify-items: center;
  align-items: center;
  gap: 30px;
  box-shadow: var(--shadow-1);
}

.header_home {
  position: absolute;
  z-index: 10;
  background-color: transparent !important;
  box-shadow: none;
  background-color: var(--primary-first);
  color: var(--primary-first);
}

.logo_header {
  margin-top: 5px;
  width: 200px;
}

h1 {
  text-align: center;
  font-family: "Italiana", serif;
  font-size: 26px;
}
</style>
