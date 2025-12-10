<script setup>
import Navigation from './components/Navigation.vue'
import Hero from './components/Hero.vue'
import Features from './components/Features.vue'
import Packages from './components/Packages.vue'
import CTA from './components/CTA.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Navigation />
  <main>
    <Hero />
    <Features />
    <Packages />
    <CTA />
  </main>
  <Footer />
</template>

<style scoped>
main {
  width: 100%;
}
</style>
