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
      heading: "Bonke Carwash Services", // Main heading of the site
      description: "Premium Carwash Services at Affordable Prices", // Hero section description
      companyName: "Bonke Carwash", // Company name used in alert
      aboutus: "At Bonke Car Wash, we provide top-notch car cleaning and detailing services to keep your vehicle looking spotless and running at its best." 
    };
  },
  methods: {
    learnMore() {
      alert(`Welcome to ${this.companyName}: ${this.aboutus}`); // Display an alert when the button is clicked
    }
  }
};
</script>

