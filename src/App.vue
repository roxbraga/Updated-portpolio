<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'
</script>

<template>
  <div id="app">
    <Navbar />

    <main>
      <Hero />
      <About />
      <Projects />
      <Skills />
      <Contact />
    </main>
  </div>
</template>