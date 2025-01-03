<template>
    <div>
      <div class="greeting-section">
        <div class="greeting-container">
          <div class="photo-container">
            <img
              src="assets/img/mey.jpg"
              alt="Kepala Sekolah"
              class="headmaster-photo"
            />
          </div>
          <table>
        <tr>
          <th>Nama </th>
          <td>Meydiana Eka Putri</td>
        </tr>
        <tr>
          <th>Alamat</th>
          <td>Kp.Cidahu Sukajaya, Kecamatan Purbaratu, Kota Tasikmalaya</td>
        </tr>
        <tr>
          <th>Tempat Tanggal lahir</th>
          <td>Kuningan, 12 Mei 20077</td>
        </tr>
      </table>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
      };
    },
  };
  </script>
  
  <style scoped>

table {
  width: 100%;
  border-collapse: collapse;
  margin: 1rem 0;
}

th, td {
  border: 1px solid #ddd;
  padding: 12px;
  text-align: left;
}

th {
  background-color: #f2f2f2;
}

tr:nth-child(even) {
  background-color: #f9f9f9; 
}

tr:hover {
  background-color: #e0f7fa; 
}

nav {
  margin-bottom: 1rem;
}

nav a {
  margin-right: 15px;
  text-decoration: none;
  color: #007bff;
  font-weight: 500;
}

nav a:hover {
  text-decoration: underline;
}

td {
  padding-left: 20px; 
}

p {
  margin-bottom: 1rem;
}
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
  