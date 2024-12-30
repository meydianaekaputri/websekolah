<template>
  <div class="container">
    <h1>Daftar Ekstrakurikuler</h1>
    <div class="card-container">
      <div v-for="ekskul in ekstrakurikuler" :key="ekskul.id" class="card">
        <h3>{{ ekskul.nama }}</h3>
        <p>{{ ekskul.deskripsi }}</p>
        <button class="btn-detail">Detail</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const ekstrakurikuler = ref([
  { id: 1, nama: 'PASKIBRA', deskripsi: 'Gerakan kepanduan.' },
  { id: 3, nama: 'FUTSAL', deskripsi: 'Olahraga sepak bola dalam ruangan.' },
  { id: 4, nama: 'PKS', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'PMR', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'VOLLY', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'ENGLISH CLUB', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'IT CLUB', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'ROHIS', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'BASKET', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'CINEMATOGRAPHY', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: '', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
  { id: 4, nama: 'Karya Ilmiah Remaja', deskripsi: 'Kelompok penelitian dan inovasi.' },
])
</script>

<style scoped>
.container {
  max-width: 1200px;
  margin: auto;
  padding: 20px;
  text-align: center;
}

h1 {
  margin-bottom: 30px;
  color: #333;
}

.card-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

.card {
  background: #ffffff;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 20px;
  text-align: left;
  transition: transform 0.2s, box-shadow 0.2s;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15);
}

h3 {
  margin: 0 0 10px;
  color: #000000;
}

p {
  color: #555;
  margin-bottom: 20px;
}

.btn-detail {
  background: rgba(35, 13, 88, 0.333);
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 15px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btn-detail:hover {
  background: #3e107a;
}
</style>
