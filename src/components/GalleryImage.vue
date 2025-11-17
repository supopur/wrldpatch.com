<template>
<div class="previewImage">
  <img :src="image" alt="Gallery Image">
</div>
</template>

<script>
export default {
  name: "GalleryImage",
  props: {
    image: {
      type: String,
    }
  }
}
</script>

<style scoped>

</style>