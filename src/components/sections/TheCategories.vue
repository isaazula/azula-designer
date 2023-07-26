<script setup></script>

<template>
  <section class="categories">
     <video class="video-categories" muted autoplay loop>
      <source src="@/assets/videos/mac.mp4" type="video/mp4" />
    </video>
    <img src="/images/image_2.jpeg" alt="Category 2" />
    <img src="/images/image_3.jpeg" alt="Category 3" />
  </section>
</template>

<style scoped>
.categories {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 70px;
  margin: 70px;
}

.categories > img {
  width: 100%;
}

.video-categories{
  width: 100%;
}
</style>
