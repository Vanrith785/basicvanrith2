<template>
  <header class="bg-white shadow sticky top-0 z-50">
    <div class="container mx-auto px-4 flex items-center justify-between py-4">
      <h1 class="text-xl font-bold">Alex Smith</h1>
      <button @click="toggleMenu" class="md:hidden text-2xl">
        <i class="bi bi-list"></i>
      </button>
      <nav :class="['md:flex gap-6 items-center', menuOpen ? 'block' : 'hidden']" class="absolute md:static bg-white top-full left-0 w-full md:w-auto p-4 md:p-0">
        <a href="#hero" class="block py-2 md:py-0 hover:text-blue-600">Home</a>
        <a href="#about" class="block py-2 md:py-0 hover:text-blue-600">About</a>
        <a href="#resume" class="block py-2 md:py-0 hover:text-blue-600">Resume</a>
        <a href="#portfolio" class="block py-2 md:py-0 hover:text-blue-600">Portfolio</a>
        <a href="#services" class="block py-2 md:py-0 hover:text-blue-600">Services</a>
        <a href="#testimonials" class="block py-2 md:py-0 hover:text-blue-600">Testimonials</a>
        <a href="#contact" class="block py-2 md:py-0 hover:text-blue-600">Contact</a>
      </nav>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'
const menuOpen = ref(false)
const toggleMenu = () => {
  menuOpen.value = !menuOpen.value
}
</script>
