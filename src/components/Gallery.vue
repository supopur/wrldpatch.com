<template>
<div class="gallery">
  <header class="gallery__header">Wassup</header>
  <div class="imgContainer">
    <GalleryImage v-for="(img, index) in images" :key="index" :image="img"></GalleryImage>
  </div>
</div>
</template>

<script>
import GalleryImage from "@/components/GalleryImage.vue";

export default {
  name: "Gallery",
  methods: {

  },
  components: {
    GalleryImage
  },
  data() {
    return {
      images: [
          "https://www.technikaizs.cz/wp-content/uploads/2025/08/P1208622-768x512.jpg",
          "https://www.technikaizs.cz/wp-content/uploads/2024/10/DSCN2082-768x512.jpg",
          "https://www.technikaizs.cz/wp-content/uploads/2025/10/IMG_8637-768x512.jpg"
      ]
    }
  }
}
</script>

<style scoped>
.imgContainer {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));

}
</style>