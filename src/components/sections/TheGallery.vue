<script setup></script>

<template>
  <section class="gallery">
    <img src="/images/image_1.jpeg" alt="Category 1" />
    <img src="/images/image_2.jpeg" alt="Category 2" />
    <img src="/images/image_3.jpeg" alt="Category 3" />
  </section>
</template>

<style scoped>
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 70px;
  margin: 70px;
}

.gallery > img {
  width: 100%;
  box-shadow: var(--shadow-3);
}
</style>
