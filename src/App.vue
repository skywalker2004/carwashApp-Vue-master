<template>
  <div>
    <div class="headersection">
      <header>
        <h1>{{ heading }}</h1>
        <nav>
          <a href="#services">Services</a>
          <a href="#about">About Us</a>
          <a href="#gallery">Gallery</a>
          <a href="#contact">Contact Us</a>
        </nav>
      </header>

      <div class="hero">
        <h2>{{ description }}</h2>
        <button @click="learnMore">Learn more</button>
      </div>
    </div>

    <section id="services">
      <ServicesComponent />
    </section>

    <section id="about">
      <AboutUs />
    </section>

    <section id="gallery">
      <GalleryComponent />
    </section>

    <section id="contact">
      <ContactUs />
    </section>

    <Footer /> <!-- Include Footer component -->
  </div>
</template>

<script>
import ServicesComponent from './components/ServicesComponent.vue';
import ContactUs from './components/ContactUs.vue';
import AboutUs from './components/AboutUs.vue';
import GalleryComponent from './components/GalleryComponent.vue';
import Footer from './components/Footer.vue'; // Import the Footer component

export default {
  name: "App",
  components: {
    ServicesComponent,
    ContactUs,
    AboutUs,
    GalleryComponent,
    Footer, // Register the Footer component
  },
  data() {
    return {
      heading: "Bonke Carwash Services",
      description: "Premium Carwash Services at Affordable Prices",
      companyName: "Bonke Carwash", 
      aboutus: "At Bonke Car Wash, we provide top-notch car cleaning and detailing services to keep your vehicle looking spotless and running at its best." 
    };
  },
  methods: {
    learnMore() {
      alert(`Welcome to ${this.companyName}: ${this.aboutus}`); 
    }
  }
};
</script>

<style scoped>
.headersection {
  background-color: #4285f4;
  text-align: center;
  padding: 20px;
  color: white;
}

header nav {
  display: flex;
  justify-content: center;
  gap: 15px;
  margin: 20px 0;
}

header nav a {
  text-decoration: none;
  color: white;
  font-size: 18px;
}

.hero {
  background-image: url('./assets/images/carwash1.jpg');
  background-size: cover;
  color: white;
  padding: 50px;
}

.hero h2 {
  font-size: 30px;
}

.hero button {
  background-color: chartreuse;
  border: none;
  padding: 15px 40px;
  border-radius: 10px;
  font-size: 18px;
}

section {
  margin: 50px 0;
}

button:hover {
  background-color: #2c3e50;
  color: white;
}
</style>
