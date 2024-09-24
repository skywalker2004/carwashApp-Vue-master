<template>
    <div class="about-us">
      <h2>About Us</h2>
      <p>{{ about }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        about: "At Bonke Car Wash, we strive to provide the best car care in town." 
      };
    }
  };
  </script>
  
  <style scoped>
  .about-us {
    padding: 30px;
    background-color: #f0f0f0;
    text-align: center;
  }
  </style>
  