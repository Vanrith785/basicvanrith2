<template>
  <section id="portfolio" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Portfolio</h2>
      <p class="text-center text-gray-600 mb-10">
        Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem.
      </p>
      <div class="grid md:grid-cols-3 gap-6">
        <div
          v-for="(item, index) in projects"
          :key="index"
          class="bg-white rounded-lg overflow-hidden shadow hover:shadow-lg transition"
        >
          <img :src="item.image" alt="project" class="w-full h-48 object-cover" />
          <div class="p-4">
            <h4 class="font-semibold text-lg mb-1">{{ item.title }}</h4>
            <p class="text-sm text-gray-500 mb-2">{{ item.category }}</p>
            <p class="text-sm text-gray-600">{{ item.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: 'App 1',
    category: 'App',
    description: 'Lorem ipsum dolor sit amet.',
    image: '/images/app-1.jpg'
  },
  {
    title: 'Product 1',
    category: 'Product',
    description: 'Adipisci atque cum quia aut.',
    image: '/images/product-1.jpg'
  },
  {
    title: 'Branding 1',
    category: 'Branding',
    description: 'Sit sint consectetur velit.',
    image: '/images/branding-1.jpg'
  },
  {
    title: 'Books 1',
    category: 'Books',
    description: 'Et nemo qui impedit suscipit.',
    image: '/images/books-1.jpg'
  },
  {
    title: 'App 2',
    category: 'App',
    description: 'Lorem ipsum dolor sit amet.',
    image: '/images/app-2.jpg'
  },
  {
    title: 'Product 2',
    category: 'Product',
    description: 'Voluptas sit aspernatur aut.',
    image: '/images/product-2.jpg'
  }
]
</script>
