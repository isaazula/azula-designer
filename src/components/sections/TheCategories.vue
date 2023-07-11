<script setup></script>

<template>
  <section class="categories">
    <img src="/src/image_1.jpeg" alt="Category 1" />
    <img src="/src/image_2.jpeg" alt="Category 2" />
    <img src="/src/image_3.jpeg" alt="Category 3" />
  </section>
</template>

<style scoped>
.categories {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 82px;
}

.categories > img {
  width: 1080px;
}
</style>
