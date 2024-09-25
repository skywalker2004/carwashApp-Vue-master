<template>
  <div class="services-section">
    <h2>Our Services</h2>
    <!-- Loop over each service using v-for and display its details -->
    <div class="service" v-for="service in services" :key="service.id">
      <h3>{{ service.name }}</h3>
      <p>{{ service.description }}</p>
      <h4>{{ service.price }} KES</h4> 
    </div>
  </div>
</template>
<script>
export default {
  name: "ServicesComponent",
  data() {
    return {
      services: [
        { id: 1, name: "Full Car Wash", description: "Complete exterior and interior wash", price: "1000" },
        { id: 2, name: "Engine Detailing", description: "Thorough engine cleaning and detailing", price: "1500" },
        { id: 3, name: "Tire & Rim Cleaning", description: "Deep tire and rim wash", price: "400" },
        { id: 4, name: "Window Tint", description: "Professional window tinting service", price: "1300" }  
      ]
    };
  }
};
</script>
