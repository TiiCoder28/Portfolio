<script setup>
import Header from './components/Header.vue';
import Home from './components/Home.vue';
import Education from './components/Education.vue';
import Services from './components/Services.vue';
import Projects from './components/Projects.vue';
</script>

<template>
  <header class="header">
    <Header />
  </header>
  <br />
  <section>
    <Home />
  </section>
  <section>
    <Education />
  </section>
  <section>
    <Services />
  </section>

  <section>
    <Projects />
  </section>
</template>

<style>

  

</style>