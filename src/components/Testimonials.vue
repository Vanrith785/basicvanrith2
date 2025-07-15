<template>
  <section id="testimonials" class="py-16 bg-white">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Testimonials</h2>
      <p class="text-center text-gray-600 mb-10"></p>
      <div class="grid md:grid-cols-3 gap-6">
        <div
          v-for="(testimonial, index) in testimonials"
          :key="index"
          class="bg-gray-100 p-6 rounded-lg shadow text-center"
        >
          <p class="italic text-sm text-gray-600 mb-4">
            "{{ testimonial.quote }}"
          </p>
          <img
            :src="testimonial.image"
            alt="photo"
            class="w-16 h-16 rounded-full mx-auto mb-2"
          />
          <h4 class="font-semibold">{{ testimonial.name }}</h4>
          <span class="text-sm text-gray-500">{{ testimonial.role }}</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const testimonials = [
  {
    name: "Rith Kimnarita",
    role: "CEO & Founder",
    quote:
      "Working with Vanrith was a great experience. He was quick, communicative, and delivered a beautiful, mobile-responsive website that exceeded our expectations.",
    image: "/images/testimonials-1.jpg",
  },
  {
    name: "Pring Mey",
    role: "Designer",
    quote:
      "Vanrith’s attention to detail and clean code made a huge difference in our project. He understood our needs clearly and executed everything perfectly..",
    image: "/images/testimonials-2.jpg",
  },
  {
    name: "Rith Sovan",
    role: "Store Owner",
    quote:
      "I’m impressed with his professionalism and speed. He turned our ideas into a working product in just a few days. Highly recommended!.",
    image: "/images/testimonials-3.jpg",
  },
];
</script>
