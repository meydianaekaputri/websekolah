<template>
  <div>
    <header>
      <h1 class="text-center">Jurusan Sekolah</h1>
    </header>

    <main class="container">
      <section>
        <h2>Daftar Jurusan</h2>
        <p>Berikut adalah daftar jurusan yang tersedia di SMKN 4 Tasikmalaya.</p>

        <!-- Display Images Only -->
        <div class="jurusan-images">
          <div v-for="jurusan in jurusanList" :key="jurusan.id" class="jurusan-item">
            <img :src="jurusan.image" alt="Foto {{ jurusan.name }}" class="jurusan-photo" />
          </div>
        </div>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // Sample data for jurusan (departments)
      jurusanList: [
        { 
          id: 1, 
          name: "Teknik Komputer dan Jaringan (TKJ)", 
          slug: "tkj",
          image: "/assets/img/tkj.jpg",  // Add image for TKJ
        },
        { 
          id: 2, 
          name: "Pengembangan Perangkat Lunak dan Gim (PPLG)", 
          slug: "rpl",
          image: "/assets/img/rpl.jpg",  // Add image for PPLG
        },
        { 
          id: 3, 
          name: "Teknik Bisnis Sepeda Motor (TBSM)", 
          slug: "tbsm",
          image: "/assets/img/tbsm.jpeg",  // Add image for TBSM
        },
        { 
          id: 4, 
          name: "Teknik Otomasi Industri (TOI)", 
          slug: "toi",
          image: "/assets/img/toi.jpg",  // Add image for TOI
        },
        { 
          id: 5, 
          name: "Desain Komunikasi Visual (DKV)", 
          slug: "dkv",
          image: "/assets/img/dkv.jpg",  // Add image for DKV
        }
      ]
    };
  }
};
</script>

<style scoped>
.jurusan-images {
  margin-top: 30px;
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: center;
}

.jurusan-item {
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Enlarging the image size */
.jurusan-photo {
  width: 350px;  /* Increase the width of the image */
  height: 350px; /* Increase the height of the image */
  object-fit: cover; /* Ensures the image maintains its aspect ratio and fills the box */
  border-radius: 10px; /* Rounded corners for a smoother look */
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2); /* Optional: shadow effect for better visibility */
}
</style>
