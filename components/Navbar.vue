<template>
  <div class="container-fluid">
    <nav class="navbar navbar-expand-lg custom-navbar"> <!-- Navbar Container -->
      <!-- Logo Section -->
      <a class="navbar-brand d-flex align-items-center" href="#">
        <img 
          src="assets/img/logo.png" 
          alt="logo SMKN 4" 
          class="img-fluid logo-image me-2"
        >
        <span class="logo-text">SMKN 4 TASIKMALAYA</span>
      </a>

      <!-- Toggle Button for Mobile View -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Navbar Items -->
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <!-- Link to Home -->
          <li class="nav-item">
            <NuxtLink class="nav-link" to="/">HOME</NuxtLink>
          </li>
          <!-- Link to Profil -->
          <li class="nav-item">
            <NuxtLink class="nav-link" to="/profil">PROFIL</NuxtLink>
          </li>
          <!-- Link to Jurusan -->
          <li class="nav-item">
            <NuxtLink class="nav-link" to="/jurusan">JURUSAN</NuxtLink>
          </li>
          <!-- Link to Ekstrakurikuler -->
          <li class="nav-item">
            <NuxtLink class="nav-link" to="/ekstrakurikuler">EKSTRAKURIKULER</NuxtLink>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<style scoped>
/* Navbar Styling */
.custom-navbar {
  background-color: #2f2546; /* Custom background color */
  padding: 10px 20px;
  width: 100%; /* Make the navbar full width */
  position: relative; /* Ensure it stays in place at the top */
  z-index: 10; /* Make sure it's above other content */
}

/* Navbar Logo Section */
.navbar-brand {
  display: flex;
  align-items: center;
}

.logo-image {
  max-height: 50px; /* Adjust logo size */
  width: auto;
}

.logo-text {
  color: #fff; /* Text color matching navbar */
  font-size: 18px;
  font-weight: 600;
  margin-left: 5px;
}

/* Navbar Items */
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
  color: #fdd835; /* Yellow hover effect */
}

/* Make Navbar Full Width */
.container-fluid {
  padding-left: 0; /* Remove padding on the left */
  padding-right: 0; /* Remove padding on the right */
}

/* Responsive Styling */
@media (max-width: 768px) {
  .logo-image {
    max-height: 40px; /* Smaller logo size for smaller screens */
  }

  .navbar-nav {
    flex-direction: column; /* Stack items vertically on smaller screens */
    gap: 10px;
  }
}
</style>
