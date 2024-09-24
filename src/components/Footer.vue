<template>
    <footer class="footer">
      <p>&copy; {{ currentYear }} Bonke Carwash. All rights reserved.</p>
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
    name: "AppFooter", // Update the name here
    data() {
      return {
        currentYear: new Date().getFullYear(),
      };
    },
  };
  </script>
  
  <style scoped>
  .footer {
    background-color: #4285f4;
    color: white;
    text-align: center;
    padding: 20px;
  }
  
  .footer nav {
    margin-top: 10px;
  }
  
  .footer nav a {
    color: white;
    margin: 0 10px;
    text-decoration: none;
  }
  
  .footer nav a:hover {
    text-decoration: underline;
  }
  </style>
  