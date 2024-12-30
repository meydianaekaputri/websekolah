<template>
  <div>
    <!-- Navbar -->
    <Navbar />

    <!-- Main Content (Slot untuk konten halaman) -->
    <slot />

    <!-- Footer -->
    <Footer />
  </div>
</template>

<script>
// Mengimpor komponen Navbar dan Footer
import Navbar from '~/components/Navbar.vue';
import Footer from '~/components/footer.vue';

export default {
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style scoped>
/* Styling untuk layout */
div {
  display: flex;
  flex-direction: column;

}

/* Styling untuk konten utama */
main {
  flex: 1;
}
</style>
