<template>
  <section id="services" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Services</h2>
      <p class="text-center text-gray-600 mb-10">
        Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem.
      </p>
      <div class="grid md:grid-cols-3 gap-6">
        <div v-for="(service, index) in services" :key="index" class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition">
          <div class="text-blue-500 text-3xl mb-3">
            <i :class="service.icon"></i>
          </div>
          <h4 class="text-xl font-semibold mb-2">{{ service.title }}</h4>
          <p class="text-sm text-gray-600">{{ service.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const services = [
  { title: "Lorem Ipsum", description: "Voluptatum deleniti atque corrupti...", icon: "bi bi-briefcase" },
  { title: "Dolor Sitema", description: "Minim veniam, quis nostrud...", icon: "bi bi-card-checklist" },
  { title: "Sed ut perspiciatis", description: "Duis aute irure dolor...", icon: "bi bi-bar-chart" },
  { title: "Magni Dolores", description: "Excepteur sint occaecat...", icon: "bi bi-binoculars" },
  { title: "Nemo Enim", description: "At vero eos et accusamus...", icon: "bi bi-brightness-high" },
  { title: "Eiusmod Tempor", description: "Et harum quidem rerum...", icon: "bi bi-calendar4-week" }
]
</script>
