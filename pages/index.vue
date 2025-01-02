<template>
  <div>
    <!-- Section for SMKN 4 Image -->
    <section class="image-section">
      <div class="image-container">
        <img
          src="assets/img/guru2.jpg"
          alt="SMKN 4"
          class="large-photo"
        />
        <!-- Text inside the image -->
        <div class="image-text">SELAMAT DATANG DI SMK PUSAT KEUNGGULAN SMKN 4 TASIKMALAYA</div>
      </div>
    </section>

    <!-- Section for Headmaster's Greeting with Photo -->
    <div class="greeting-section">
      <div class="greeting-container">
        <!-- Headmaster's Photo -->
        <div class="photo-container">
          <img
            src="assets/img/kepalaskl.jpg"
            alt="Kepala Sekolah"
            class="headmaster-photo"
          />
        </div>

        <!-- Headmaster's Greeting Text -->
        <div class="greeting-card">
          <h2>Sambutan Kepala Sekolah</h2>
          <p>
            Assalamualaikum Warahmatullahi Wabarakatuh. Selamat datang di SMKN 4 Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas perkenan-Nya pula kami dapat
            menghadirkan website SMK Negeri 4 Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4 Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang sekolah kami sehingga dapat mempererat tali silaturrahmi
            antara sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading yang tak retak, website kami ini masih dalam proses pengembangan, masih banyak kekurangan yang harus kami perbaiki. Kritik dan sarannya yang membangun
            sangat kami harapkan untuk pengembangan ke depan.
          </p>
        </div>
      </div>
    </div>

    <!-- Box Berita Section (News Box) -->
    <section class="news-section">
      <div class="news-container">
        <h3>Berita Terbaru</h3>
        <div class="news-card">
          <div class="news-header">
            <h4>Pengumuman Pendaftaran Siswa Baru</h4>
            <span class="news-date">20 Desember 2024</span>
          </div>
          <div class="news-content">
            <p>
              Pendaftaran siswa baru untuk tahun ajaran 2024/2025 sudah dibuka. Untuk informasi lebih lanjut, silakan kunjungi halaman pendaftaran di website kami atau hubungi pihak sekolah. Jangan lewatkan kesempatan untuk bergabung dengan
              SMKN 4 Tasikmalaya!
            </p>
            <NuxtLink
              to="/berita"
              class="read-more"
              >Baca Selengkapnya</NuxtLink
            >
          </div>
        </div>
        <!-- You can add more news cards here -->
      </div>
    </section>

    <main class="container">
      <section>
        <div class="table-container"></div>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // Any needed data can be added here
    };
  },
};
</script>

<style scoped>
/* Image Section */
.image-section {
  text-align: center;
  margin-top: -100px;
  padding-top: 50px;
}

.image-container {
  position: relative;
  display: inline-block;
}

.large-photo {
  width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  object-fit: cover;
}

.image-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  font-size: 2rem;
  font-weight: bold;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
  text-align: center;
}

/* Greeting Section */
.greeting-section {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 30px;
}

.greeting-container {
  max-width: 800px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  background: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.photo-container {
  margin-bottom: 20px;
}

.headmaster-photo {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 50%;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.greeting-card {
  text-align: center;
}

.greeting-card h2 {
  margin-top: 0;
  font-size: 1.8rem;
  color: #007bff;
}

.greeting-card p {
  font-size: 1rem;
  color: #333;
  line-height: 1.6;
  margin-top: 10px;
  text-align: justify;
}

/* News Box (Box Berita) Section */
.news-section {
  margin-top: 50px;
  padding: 20px;
  background: #f1f1f1;
  border-radius: 8px;
}

.news-container h3 {
  font-size: 2rem;
  text-align: center;
  color: #333;
  margin-bottom: 20px;
}

.news-card {
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
}

.news-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 10px;
}

.news-header h4 {
  font-size: 1.6rem;
  color: #333;
}

.news-date {
  font-size: 0.9rem;
  color: #777;
}

.news-content p {
  font-size: 1rem;
  color: #333;
  line-height: 1.6;
  margin-bottom: 10px;
}

.read-more {
  font-size: 1rem;
  color: #007bff;
  text-decoration: none;
}

.read-more:hover {
  text-decoration: underline;
}

/* Responsive Design */
@media (max-width: 768px) {
  .large-photo {
    width: 100%;
    height: 50%;
  }

  .headmaster-photo {
    width: 120px;
    height: 120px;
  }

  .greeting-container {
    padding: 15px;
  }

  .greeting-card h2 {
    font-size: 1.5rem;
  }

  .greeting-card p {
    font-size: 0.95rem;
  }

  .news-container h3 {
    font-size: 1.5rem;
  }

  .news-card {
    padding: 15px;
  }

  .news-header h4 {
    font-size: 1.4rem;
  }

  .news-date {
    font-size: 0.8rem;
  }

  .news-content p {
    font-size: 0.95rem;
  }

  .read-more {
    font-size: 0.95rem;
  }
}
</style>
