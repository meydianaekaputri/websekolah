<template>
  <div>
    <section class="image-section">
      <img src="assets/img/smkn4.jpg" alt="SMKN 4" class="large-photo" />
    </section>

    <section class="welcome-card">
      <div class="card">
        <h2>Sambutan Kepala Sekolah</h2>
        <p>
          Assalamu'alaikum warahmatullahi wabarakatuh, <br />
          Selamat datang di website resmi SMKN 4. Kami berkomitmen untuk menyediakan pendidikan berkualitas dan membentuk generasi muda yang berprestasi, kreatif, dan berkarakter. Semoga informasi yang ada di website ini dapat bermanfaat bagi kita semua.
        </p>
        <p>
          Hormat kami,<br />
          <strong>Drs. Agus Priyanto, M.Pd.</strong><br />
          Kepala Sekolah
        </p>
      </div>
    </section>

    <main class="container">
      <section>
        <div class="table-container"></div>
      </section>
    </main>
  </div>
</template>

<style scoped>
.image-section {
  text-align: center;
}

.large-photo {
  width: 100%;
  max-width: 1000px; 
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); 
}

.welcome-card {
  display: flex;
  justify-content: center;
  margin-top: 20px;
  padding: 0 20px;
}

.card {
  max-width: 800px;
  background: #ffffff;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 20px;
  text-align: left;
  line-height: 1.6;
  color: #333;
}

.card h2 {
  margin-top: 0;
  font-size: 1.8rem;
  color: #007BFF;
}

.card p {
  margin: 10px 0;
}

.table-container {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.photo-table {
  border-collapse: collapse;
  width: 80%;
}

.photo-table td {
  padding: 10px;
  text-align: center;
}

.photo-table .photo {
  width: 100%;
  height: auto;
  max-width: 150px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); 
}

@media (max-width: 768px) {
  .photo-table {
    width: 100%;
  }

  .photo-table td {
    display: inline-block;
    width: 100%;
    padding: 5px;
  }

  .photo-table .photo {
    max-width: 100%;
  }

  .large-photo {
    width: 100%; 
    max-width: 100%;
  }

  .welcome-card {
    padding: 0 10px;
  }

  .card {
    padding: 15px;
  }
}
</style>
