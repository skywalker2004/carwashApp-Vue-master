<template>
  <div class="galleryComponent">
    <h2>Our Gallery</h2> <!-- Gallery section heading -->
    <div class="images">
      <!-- Two sample images for the gallery -->
      <img src="@/assets/images/carwash1.jpg" alt="Car wash 1" />
      <img src="@/assets/images/carwash2.jpg" alt="Car wash 2" />
    </div>
  </div>
</template>
<script>
export default {
  name: "GalleryComponent", // Register the component name
};
</script>
<style scoped>
/* Center the gallery content */
.galleryComponent {
  text-align: center; 
}

/* Arrange images horizontally with flexbox */
.images {
  display: flex;
  justify-content: center; /* Center the images horizontally */
  gap: 20px; /* Add space between the images */
}

/* Style individual images */
.images img {
  width: 300px; /* Set fixed width for each image */
  border-radius: 10px; /* Rounded corners for the images */
}
</style>

