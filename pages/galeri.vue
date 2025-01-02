<template>
  <div class="gallery-container">
    <h1>Galeri Sekolah</h1>
    <div class="gallery-grid">
      <div class="gallery-item">
        <img
          src="~/assets/img/tbsm.jpg"
          alt="Gambar 1"
          class="gallery-image"
        />
        <p>Deskripsi Gambar 1</p>
      </div>
      <div class="gallery-item">
        <img
          src="~/assets/img/tbsm.jpg"
          alt="Gambar 2"
          class="gallery-image"
        />
        <p>Deskripsi Gambar 2</p>
      </div>
      <div class="gallery-item">
        <img
          src="~/assets/img/tbsm.jpg"
          alt="Gambar 3"
          class="gallery-image"
        />
        <p>Deskripsi Gambar 3</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Gallery',
};
</script>

<style scoped>
.gallery-container {
  text-align: center;
  margin: 20px;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.gallery-item {
  border: 2px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  text-align: center;
}

.gallery-image {
  width: 100%;
  height: auto;
  border-bottom: 2px solid #ddd;
}

.gallery-item p {
  padding: 10px;
  font-size: 1rem;
  color: #333;
  background-color: #f9f9f9;
  margin: 0;
}
</style>
