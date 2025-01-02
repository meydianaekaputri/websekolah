<template>
  <div class="jurusan-container">
    <header class="page-header">
      <h1 class="text-center">Daftar Ekstrakurikuler SMKN 4 Tasikmalaya</h1>
    </header>

    <main class="container">
      <section>
        <div class="row mt-3 m-3 justify-content-center">
          <div class="col-md-3">
            <div class="card">
              <img
                src="~/assets/img/tkj.jpeg"
                alt="logo"
                class="mt-3"
              />
              <div class="card-body">
                <h5 class="text-center">MPK</h5>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="card">
              <img
                src="~/assets/img/rpl.jpeg"
                alt="logo"
                class="mt-3"
              />
              <div class="card-body">
                <h5 class="text-center mt-1">OSIS</h5>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="card">
              <img
                src="~/assets/img/tsmlogo.jpeg"
                alt="logo"
                class="mt-3"
              />
              <div class="card-body">
                <h5 class="text-center mt-3">PUB</h5>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
  </div>

  <!-- Display Departments in Boxes -->
  <!-- <div class="jurusan-boxes">
          <div
            v-for="jurusan in jurusanList"
            :key="jurusan.id"
            class="jurusan-box"
          >
            <img
              :src="jurusan.image"
              :alt="'Foto ' + jurusan.name"
              class="jurusan-image"
            />
            <div class="jurusan-info">
              <h3 class="jurusan-title">{{ jurusan.name }}</h3>
              <p class="jurusan-description">{{ jurusan.description }}</p>
            </div>
          </div>
        </div> -->
</template>

<style scoped>
.container-fluid {
  margin-top: 115px;
}

img {
  width: 200px;
  margin: auto;
}
</style>
<!-- <script>
export default {
  data() {
    return {
      // Sample data for jurusan (departments)
      jurusanList: [
        {
          id: 1,
          name: 'Teknik Komputer dan Jaringan (TKJ)',
          description: 'Jurusan yang mempelajari tentang jaringan komputer dan infrastruktur IT.',
          image: '/assets/img/tkj.jpeg', // Image path
        },
        {
          id: 2,
          name: 'Pengembangan Perangkat Lunak dan Gim (PPLG)',
          description: 'Jurusan untuk pengembangan perangkat lunak dan game.',
          image: '/assets/images/rpl.jpg', // Image path
        },
        {
          id: 3,
          name: 'Teknik Bisnis Sepeda Motor (TBSM)',
          description: 'Jurusan yang mempelajari tentang perawatan dan reparasi sepeda motor.',
          image: '/assets/images/tbsm.jpg', // Image path
        },
        {
          id: 4,
          name: 'Teknik Otomasi Industri (TOI)',
          description: 'Jurusan yang mengajarkan teknik otomasi dalam industri.',
          image: '/assets/images/toi.jpg', // Image path
        },
        {
          id: 5,
          name: 'Desain Komunikasi Visual (DKV)',
          description: 'Jurusan yang mempelajari desain grafis dan komunikasi visual.',
          image: '/assets/images/dkv.jpg', // Image path
        },
      ],
    };
  },
};
</script> -->

<!-- <style scoped>
/* Styling for the container */
.jurusan-container {
  margin: 0 auto;
  padding: 20px;
  max-width: 1200px;
}

/* Page Header Styling */
.page-header {
  text-align: center;
  margin-bottom: 40px;
}

.page-header h1 {
  font-size: 36px;
  color: #2f2546;
  font-weight: bold;
}

/* Section Title and Description */
.section-title {
  font-size: 24px;
  text-align: center;
  margin-top: 20px;
}

.section-description {
  text-align: center;
  color: #555;
  font-size: 16px;
  margin-bottom: 30px;
}

/* Box layout for jurusan items */
.jurusan-boxes {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

/* Styling for each jurusan box */
.jurusan-box {
  width: 250px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  text-align: center;
}

.jurusan-box:hover {
  transform: scale(1.05); /* Slight scaling effect on hover */
}

/* Image styling */
.jurusan-image {
  width: 100%;
  height: 180px;
  object-fit: cover; /* Ensures the image covers the entire box without distortion */
}

/* Styling for the info inside the box */
.jurusan-info {
  padding: 15px;
}

.jurusan-title {
  font-size: 18px;
  font-weight: bold;
  color: #333;
  margin: 10px 0;
}

.jurusan-description {
  font-size: 14px;
  color: #777;
}

/* Responsive Design for smaller screens */
@media (max-width: 768px) {
  .jurusan-box {
    width: 100%; /* Make the boxes full width on smaller screens */
  }

  .jurusan-image {
    height: 150px; /* Reduce image height for smaller screens */
  }
}
</style> -->
