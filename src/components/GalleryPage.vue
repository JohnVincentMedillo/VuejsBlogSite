<template>
  <div class="gallery">
    <h1>My Gallery</h1>
    <div class="image-grid">
      <!-- Image cards -->
      <div class="image-card">
        <img src="@/assets/gal1.webp" alt="Image 1">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal2.webp" alt="Image 2">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal3.webp" alt="Image 3">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal4.webp" alt="Image 4">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal5.webp" alt="Image 5">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal6.webp" alt="Image 6">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal7.webp" alt="Image 7">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal8.webp" alt="Image 8">
        <div class="overlay"></div>
      </div>
      <div class="image-card">
        <img src="@/assets/gal9.webp" alt="Image 9">
        <div class="overlay"></div>
      </div>
     
    </div>
  </div>
</template>

<script>
export default {
  name: 'GalleryPage',
}
</script>

<style scoped>
.gallery {
  padding: 50px;
  text-align: center;
  background-image: url('@/assets/bembg.png');
  background-size: cover;
  background-attachment: fixed; /* Fixed background */
}

.image-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
}

.image-card {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  height: 300px; /* Set a fixed height for all image cards */
}

.image-card img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensure the image covers the entire box */
  display: block;
  transition: transform 0.3s;
}

.image-card:hover img {
  transform: scale(1.1);
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  opacity: 0;
  transition: opacity 0.3s;
}

.image-card:hover .overlay {
  opacity: 1;
}

</style>
