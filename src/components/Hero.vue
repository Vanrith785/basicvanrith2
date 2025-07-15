<template>
  <section
    id="hero"
    class="relative h-screen flex items-center justify-left text-white text-center bg-cover bg-center"
    style="background-image: url('/images/hero-bg.jpg')"
  >
    <div class="absolute inset-0 bg-black/60 z-10"></div>
    <div class="relative z-20">
      <h1 class="text-4xl md:text-5xl font-bold mb-4">Pich Vanrith</h1>
      <p class="text-xl md:text-2xl">
        I'm <span class="text-blue-400 font-semibold" ref="typedEl"></span>
      </p>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import Typed from 'typed.js'

const typedEl = ref(null)

onMounted(() => {
  new Typed(typedEl.value, {
    strings: ['Designer', 'Developer', 'Freelancer', 'Photographer'],
    typeSpeed: 60,
    backSpeed: 30,
    backDelay: 1200,
    loop: true
  })
})
</script>

