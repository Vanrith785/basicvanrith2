<template>
  <section id="contact" class="py-16 bg-white">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Contact</h2>
      <p class="text-center text-gray-600 mb-10">
      
      </p>

      <div class="grid md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="flex items-start gap-4">
            <i class="bi bi-geo-alt text-2xl text-blue-600"></i>
            <div>
              <h4 class="font-semibold">Address</h4>
              <p class="text-sm text-gray-600">
                #38, Street 62, Phnom Penh, Cambodia
              </p>
            </div>
          </div>
          <div class="flex items-start gap-4">
            <i class="bi bi-telephone text-2xl text-blue-600"></i>
            <div>
              <h4 class="font-semibold">Call Us</h4>
              <p class="text-sm text-gray-600">+855 81 585 785</p>
            </div>
          </div>
          <div class="flex items-start gap-4">
            <i class="bi bi-envelope text-2xl text-blue-600"></i>
            <div>
              <h4 class="font-semibold">Email Us</h4>
              <p class="text-sm text-gray-600">pichvanrith785.gmail.com</p>
            </div>
          </div>
        </div>

        <form @submit.prevent class="space-y-4">
          <div class="grid md:grid-cols-2 gap-4">
            <input
              type="text"
              placeholder="Your Name"
              class="w-full p-3 border rounded"
              required
            />
            <input
              type="email"
              placeholder="Your Email"
              class="w-full p-3 border rounded"
              required
            />
          </div>
          <input
            type="text"
            placeholder="Subject"
            class="w-full p-3 border rounded"
            required
          />
          <textarea
            rows="6"
            placeholder="Message"
            class="w-full p-3 border rounded"
            required
          ></textarea>
          <button
            type="submit"
            class="bg-blue-600 text-white px-6 py-2 rounded hover:bg-blue-700"
          >
            Send Message
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<script setup>
// Static form - no back-end handling yet
</script>
