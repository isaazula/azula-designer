<script setup>
import { useRouter, useRoute } from "vue-router";
import { onBeforeMount } from "vue";
import GalleryItem from "./GalleryItem.vue";
import { db } from "./../../lib/db";

const router = useRouter();
const route = useRoute();

onBeforeMount(() => {
  console.log(db);
});
</script>

<template>
  <section class="gallery">
    <GalleryItem v-for="(item, i) in db" :key="i" :item="item" />
  </section>
</template>

<style scoped>
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 70px;
  margin: 70px;
}
</style>
