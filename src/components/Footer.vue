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
<style scoped>
/* Footer container styling */
.footer {
  background-color: #4285f4; /* Blue background color */
  color: white; /* White text color */
  text-align: center; /* Center-align text */
  padding: 20px; /* Padding around the footer */
}

/* Navigation styles within the footer */
.footer nav {
  margin-top: 10px; /* Space between the text and navigation */
}

/* Footer link styles */
.footer nav a {
  color: white; /* White text color for links */
  margin: 0 10px; /* Add spacing between links */
  text-decoration: none; /* Remove underline from links */
}

/* Hover effect for navigation links */
.footer nav a:hover {
  text-decoration: underline; /* Underline links on hover */
}
</style>
