<script setup></script>

<template>
  <section class="categories">
    <video class="video-categories" id="v2" key="v2" muted autoplay loop>
      <source src="@/assets/videos/second.mp4" type="video/mp4" />
    </video>

    <video class="video-categories" id="v3" key="v3" muted autoplay loop>
      <source src="@/assets/videos/third.mp4" type="video/mp4" />
    </video>

    <video class="video-categories" id="v1" key="v1" muted autoplay loop>
      <source src="@/assets/videos/first.mp4" type="video/mp4" />
    </video>
  </section>
</template>

<style scoped>
.categories {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 70px;
  margin: 70px;
}

.categories > img,
video {
  width: 100%;
  height: 100%;
  box-shadow: var(--shadow-3);
}

.video-categories {
  width: 100%;
}
</style>
