<template>
  <div class="container-fluid">
    <nav class="navbar navbar-expand-lg custom-navbar">
      <a
        class="navbar-brand d-flex align-items-center"
        href="#"
      >
        <img
          src="assets/img/logo.png"
          alt="logo SMKN 4"
          class="img-fluid logo-image me-2"
        />
        <span class="logo-text">SMKN 4 TASIKMALAYA</span>
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div
        class="collapse navbar-collapse"
        id="navbarNav"
      >
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="/"
              >HOME</NuxtLink
            >
          </li>
    
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="/profil"
              >PROFIL</NuxtLink
            >
          </li>
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="/jurusan"
              >JURUSAN</NuxtLink
            >
          </li>
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="./ekskul"
              >EKSTRAKURIKULER</NuxtLink
            >
          </li>
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="/galeri"
              >GALERI</NuxtLink
            >

          </li>
          <li class="nav-item">
            <NuxtLink
              class="nav-link"
              to="/about"
              >ABOUT</NuxtLink
            >
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<style scoped>
.custom-navbar {
  background-color: #2f2546; 
  padding: 10px 20px;
  width: 100%;
  position: relative;
  z-index: 10; 
}

.navbar-brand {
  display: flex;
  align-items: center;
}

.logo-image {
  max-height: 50px; 
  width: auto;
}

.logo-text {
  color: #fff; 
  font-size: 18px;
  font-weight: 600;
  margin-left: 5px;
}

.navbar-nav {
  gap: 15px;
}

.navbar-nav .nav-link {
  color: #fff;
  font-weight: 500;
  padding: 5px 10px;
  text-decoration: none;
  transition: color 0.3s ease;
}

.navbar-nav .nav-link:hover {
  color: #fdd835; 
}

.container-fluid {
  padding-left: 0; 
  padding-right: 0; 
}

@media (max-width: 768px) {
  .logo-image {
    max-height: 40px; 
  }

  .navbar-nav {
    flex-direction: column;
    gap: 10px;
  }
}
</style>
