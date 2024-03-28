<template>
  <div>
    <h1 class="text-3xl font-bold">{{ blog.title }}</h1>
    <p>{{ blog.description }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { fetch } from '@nuxt/content'

const route = useRoute()

const blog = ref(null)

fetch(route.params.slug, { deep: true })
  .then((result) => {
    blog.value = result
  })
  .catch((error) => {
    console.error('Error fetching blog:', error)
  })
</script>
