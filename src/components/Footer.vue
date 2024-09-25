<template>
  <footer class="footer">
    <!-- Dynamic copyright year -->
    <p>&copy; {{ currentYear }} Bonke Carwash. All rights reserved.</p>
    <!-- Footer navigation -->
    <nav>
      <a href="#services">Services</a>
      <a href="#about">About Us</a>
      <a href="#gallery">Gallery</a>
      <a href="#contact">Contact Us</a>
    </nav>
  </footer>
</template>
<script>
export default {
  name: "AppFooter", // Register the component name as AppFooter
  data() {
    return {
      currentYear: new Date().getFullYear(), // Get the current year
    };
  },
};
</script>
