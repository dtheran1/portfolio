<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="bg-gradient-to-r from-cyan-500 to-blue-500">
    <Nav />
    <RouterView />
    <Footer />
  </div>
</template>
