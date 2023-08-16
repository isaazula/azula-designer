<script setup>
const props = defineProps({
  item: {
    type: Object,
    default: () => {},
  },
});

let path = `/images/${props.item.image[0]}`;
let link = `${props.item.link}`;
</script>

<template class="gallery">
  <a :href="link" target="_blank"> <img :src="path" /></a>
</template>

<style scoped>
.gallery img {
  width: 100%;
  box-shadow: var(--shadow-3);
}
</style>
