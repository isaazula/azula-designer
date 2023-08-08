<script setup></script>

<template>
  <section class="gallery">
    <a
      href="https://www.behance.net/gallery/176540355/Movie-Poster"
      target="_blank"
    >
      <img src="/images/movie.png" alt="Movie Poster"
    /></a>
    <img src="/images/caperucita.png" alt="Category 2" />
    <img src="/images/2.jpg" alt="Category 3" />
  </section>
</template>

<style scoped>
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 70px;
  margin: 70px;
}

.gallery img {
  width: 100%;
  box-shadow: var(--shadow-3);
}
</style>
