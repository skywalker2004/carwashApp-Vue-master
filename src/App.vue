<template>
  <div>
    <!-- Header section starts -->
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

      <!-- Hero section with a button -->
      <div class="hero">
        <h2>{{ description }}</h2>
        <button @click="learnMore">Learn more</button>
      </div>
    </div>

    <!-- Section for services -->
    <section id="services">
      <ServicesComponent />
    </section>

    <!-- Section for About Us -->
    <section id="about">
      <AboutUs />
    </section>

    <!-- Section for Gallery -->
    <section id="gallery">
      <GalleryComponent />
    </section>

    <!-- Section for Contact Us -->
    <section id="contact">
      <ContactUs />
    </section>

    <!-- Footer component -->
    <Footer />
  </div>
</template>
