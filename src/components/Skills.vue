<template>
  <section id="skills" class="py-16 bg-gray-50">
    <div class="container mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-6">Skills</h2>
      <p class="text-center text-gray-600 mb-10">
       
      </p>
      <div class="grid md:grid-cols-2 gap-8">
        <div v-for="skill in leftSkills" :key="skill.name">
          <div class="mb-4">
            <div class="flex justify-between mb-1">
              <span>{{ skill.name }}</span>
              <span>{{ skill.value }}%</span>
            </div>
            <div class="w-full bg-gray-300 h-2 rounded">
              <div
                class="bg-blue-500 h-2 rounded"
                :style="{ width: skill.value + '%' }"
              ></div>
            </div>
          </div>
        </div>
        <div v-for="skill in rightSkills" :key="skill.name">
          <div class="mb-4">
            <div class="flex justify-between mb-1">
              <span>{{ skill.name }}</span>
              <span>{{ skill.value }}%</span>
            </div>
            <div class="w-full bg-gray-300 h-2 rounded">
              <div
                class="bg-blue-500 h-2 rounded"
                :style="{ width: skill.value + '%' }"
              ></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const leftSkills = [
  { name: "HTML", value: 100 },
  { name: "CSS", value: 90 },
  { name: "JavaScript", value: 75 },
];

const rightSkills = [
  { name: "PHP", value: 80 },
  { name: "WordPress/CMS", value: 90 },
  { name: "Photoshop", value: 55 },
];
</script>
