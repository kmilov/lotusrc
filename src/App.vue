<script setup>
import {
  Hero,
  Services,
  CustomerReviews,
  Footer,
  About,
  Contact
} from './sections'

import Nav from './components/Nav.vue'

</script>
<template>
  <main>
    <Nav />
    
    <section class="xl:padding-l wide:padding-r">
      <Hero />
    </section>

    <section id="about" class="xl:padding-l wide:padding-r">
      <About />
    </section>

    <section id="services" class="padding">
      <Services />
    </section>

    <section id="customer" class="bg-pale-blue padding">
      <CustomerReviews />
    </section>


    <section id="contact" class="padding-x sm:py-32 py-16 w-full">
      <Contact />
    </section>

    <section class="padding-x bg-lt-black padding-t pb-8">
      <Footer />
    </section>
  </main>
</template>