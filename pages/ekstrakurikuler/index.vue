<template>
  <div class="extracurricular-container">
    <h1 class="text-center">Ekstrakurikuler di SMKN 4 Tasikmalaya</h1>
    <p class="text-center">Berikut adalah daftar kegiatan ekstrakurikuler yang tersedia di sekolah kami.</p>
    
    <!-- Extracurricular Boxes -->
    <div class="box-container">
      <div v-for="(activity, index) in extracurricularActivities" :key="index" class="box">
        <img :src="activity.image" :alt="activity.name" class="box-image" />
        <div class="box-content">
          <h3 class="box-title">{{ activity.name }}</h3>
          <p class="box-description">{{ activity.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      extracurricularActivities: [
        {
          name: 'Pramuka',
          description: 'Kegiatan kepramukaan yang membangun karakter dan kepemimpinan.',
          image: '~/assets/img/basket2.jpg' // Correct path
        },
        {
          name: 'Basket',
          description: 'Tim basket yang aktif berkompetisi dan mengasah keterampilan olahraga.',
          image: '/images/basket2.jpg', // Correct path
        },
        {
          name: 'MPR',
          description: 'Ekstrakurikuler paduan suara yang mengasah bakat di bidang musik dan seni suara.',
          image: '/images/paduan-suara.jpg', // Correct path
        },
        {
          name: 'Robotika',
          description: 'Klub robotika yang mengajarkan pembuatan dan pengoperasian robot.',
          image: '/images/robotika.jpg', // Correct path
        },
        {
          name: 'Teater',
          description: 'Kelompok seni teater yang mengembangkan bakat akting dan seni pertunjukan.',
          image: '/images/teater.jpg', // Correct path
        },
      ]
    };
  }
};
</script>

<style scoped>
/* Container for the entire extracurricular page */
.extracurricular-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
}

/* Styling for the boxes container */
.box-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
  margin-top: 30px;
}

/* Individual box styling */
.box {
  background-color: #fff;
  border: 2px solid #ddd;  /* Add a border for box effect */
  padding: 20px;
  transition: transform 0.3s ease;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

/* Box hover effect */
.box:hover {
  transform: translateY(-5px);  /* Slight hover effect */
}

/* Image styling inside box */
.box-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-bottom: 2px solid #ccc;
}

/* Box content (title and description) */
.box-content {
  padding: 15px;
  flex-grow: 1;  /* Ensure content section fills available space */
}

.box-title {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 10px;
  color: #333;
}

.box-description {
  font-size: 16px;
  color: #555;
}

/* Responsive Design */
@media (max-width: 768px) {
  .box-title {
    font-size: 18px;
  }

  .box-description {
    font-size: 14px;
  }
}
</style>
