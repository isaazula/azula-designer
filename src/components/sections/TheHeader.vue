<script setup></script>

<template>
  <header class="header_home">
    <div>
      <h1>About me</h1>
    </div>
    <div>
      <img class="logo_header" src="@/assets/images/azula.svg" alt="Logo" />
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
header {
  height: 100px;
  background-color: var(--primary-first);
  width: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  justify-items: center;
  align-items: center;
  gap: 30px;
}

.header_home {
  position: absolute;
  z-index: 10;
  background-color: transparent !important;
}

.logo_header {
  margin-top: 30px;
  width: 300px;
}

h1 {
  color: var(--color-white);
  text-align: center;
  font-family: "GFS Didot", serif;
  font-size: 26px;
}
</style>
