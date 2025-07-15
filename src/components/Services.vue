<template>
  <section id="services" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Services</h2>
      <p class="text-center text-gray-600 mb-10">
      
      </p>
      <div class="grid md:grid-cols-3 gap-6">
        <div
          v-for="(service, index) in services"
          :key="index"
          class="bg-white p-6 rounded-lg shadow hover:shadow-lg transition"
        >
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
  {
    title: "Web Design",
    description: "Design user-friendly interfaces that are both functional and attractive.",
    icon: "bi bi-briefcase",
  },
  {
    title: "Web Development",
    description: "Build responsive and modern websites using Vue.js, HTML, CSS, and JavaScript.",
    icon: "bi bi-card-checklist",
  },
  {
    title: "SEO",
    description: "I optimize websites for search engines to improve visibility and performance.",
    icon: "bi bi-bar-chart",
  },
  {
    title: "Digital Marketing",
    description: "I create layouts that look and function beautifully across all devices, from smartphones to desktops.",
    icon: "bi bi-binoculars",
  },
 
  
];
</script>
