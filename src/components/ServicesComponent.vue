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
