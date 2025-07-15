<template>
  <section id="testimonials" class="py-16 bg-white">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Testimonials</h2>
      <p class="text-center text-gray-600 mb-10">
        Necessitatibus eius consequatur ex aliquid fuga eum quidem sint consectetur velit
      </p>
      <div class="grid md:grid-cols-3 gap-6">
        <div v-for="(testimonial, index) in testimonials" :key="index" class="bg-gray-100 p-6 rounded-lg shadow text-center">
          <p class="italic text-sm text-gray-600 mb-4">"{{ testimonial.quote }}"</p>
          <img :src="testimonial.image" alt="photo" class="w-16 h-16 rounded-full mx-auto mb-2" />
          <h4 class="font-semibold">{{ testimonial.name }}</h4>
          <span class="text-sm text-gray-500">{{ testimonial.role }}</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const testimonials = [
  { name: "Saul Goodman", role: "CEO & Founder", quote: "Proin iaculis purus consequat...", image: "/images/testimonials-1.jpg" },
  { name: "Sara Wilsson", role: "Designer", quote: "Export tempor illum tamen...", image: "/images/testimonials-2.jpg" },
  { name: "Jena Karlis", role: "Store Owner", quote: "Enim nisi quem export duis...", image: "/images/testimonials-3.jpg" }
]
</script>
