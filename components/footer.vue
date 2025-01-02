<template>
  <footer class="footer">
    <div class="footer-container">
      <p>&copy; Copyright SMKN4 TASIKMALAYA.All rights reserved.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style scoped>
.footer {
  background-color: #2c3e50; /* Warna latar belakang */
  color: white; /* Warna teks */
  padding: 20px;
  text-align: center;
  margin-top: 40px;
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
}

.footer-nav {
  list-style: none;
  padding: 0;
}

.footer-nav li {
  display: inline;
  margin: 0 15px;
}

.footer-nav a {
  color: white;
  text-decoration: none;
}

.footer-nav a:hover {
  text-decoration: underline;
}
</style>
