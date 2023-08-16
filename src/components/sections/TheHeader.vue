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
      <p>AZULA</p>
    </div>
    <h1 id="menu__button">My projects</h1>
    <!-- <nav id="nav__small">
      <p class="text__nav">Branding & Packaging</p>
      <p class="text__nav">Illustrations & Prints</p>
      <p class="text__nav">Photographs & Audiovisual Content</p>
      <p class="text__nav">3D Modelling & Animations</p>
    </nav>-->
  </header>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Italiana&display=swap");

header {
  color: var(--color-white);
  height: 120px;
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

p {
  text-align: center;
  font-size: 50px;
  font-family: Didot;
  letter-spacing: 7px;
  margin-top: 5px;
}

h1 {
  text-align: center;
  font-family: "Italiana", serif;
  font-size: 26px;
  color: var(--primary-third);
}

#nav__small {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 15px;
  width: 100%;
  z-index: 9 !important;
  position: absolute;
  top: 100px;
  left: 0px;
  transition: all 0.5s;
  color: var(--primary-third);
}

.text__nav {
  font-family: Didot;
  color: var(--primary-first);
  font-size: 20px;
  letter-spacing: 0px;
  text-align: center;
  margin-left: 980px;
}
</style>
