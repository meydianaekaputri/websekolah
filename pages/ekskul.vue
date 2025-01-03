<template>
  <div class="gallery-container">
    <h1>EKSTRAKURIKULER</h1>
    <div class="gallery-grid">
      <div class="gallery-item">
        <img
          src="~/assets/img/mpk.jpeg"
          alt="Gambar 1"
          class="gallery-image"/>
        <p>MPK</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/pub.png"
          alt="Gambar 2"
          class="gallery-image"/>
        <p>PUB</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/pks.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>PKS</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/pmr.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>PMR</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/paskibra.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>PASKIBRA</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/futsal.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>FUTSAL</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/basket.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>BASKET</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/englishclub.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>ENGLISH CLUB</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/bulutangkis.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>BULU TANGKKIS</p>
      </div>

      <div class="gallery-item">
        <img
          src="~/assets/img/laskarpustaka.png"
          alt="Gambar 3"
          class="gallery-image"/>
        <p>LASKAR PUSTAKA</p>
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
