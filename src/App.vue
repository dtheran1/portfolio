<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="image">
    <Nav />
    <RouterView />
    <Footer />
  </div>
</template>

<style>
.image {
  background-image: url("./assets/IMG_20221231_220433_692.jpg"),
}
</style>
