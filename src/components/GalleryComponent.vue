<template>
  <div class="galleryComponent">
    <h2>Our Gallery</h2>
    <div class="images">
      <img src="@/assets/images/carwash1.jpg" alt="Car wash 1" />
      <img src="@/assets/images/carwash2.jpg" alt="Car wash 2" />
    </div>
  </div>
</template>

<script>
export default {
  name: "GalleryComponent", 
};
</script>

<style scoped>
.galleryComponent {
  text-align: center;
}

.images {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.images img {
  width: 300px;
  border-radius: 10px;
}
</style>