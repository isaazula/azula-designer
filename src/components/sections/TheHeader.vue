<script setup></script>

<template>
  <header class="header_home">
    <div>
      <h1>About me</h1>
    </div>
    <div>
      <img class="logo_header" src="images/azula.svg" alt="Logo" />
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
  height: 130px;
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
}

.logo_header {
  margin-top: 30px;
  width: 300px;
}

h1 {
  color: var(--color-white);
  text-align: center;
  font-family: "Italiana", serif;
  font-size: 26px;
}
</style>
