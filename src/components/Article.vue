<script setup>
import { ref } from 'vue'

const count = ref(0)
defineProps(['title', 'slug'])


const routes = [
  { 
    name: 'Article',
    path: '/article/:slug',
    component: () => import('@/views/Article.vue'),
    props:true
  }
]

</script>

<template>
      <h4>{{ title }}--{{ slug }}**</h4>
      <router-link :to="{ name: 'Article', params: { slug: slug }}">{{ title }}</router-link>
  <button @click="count++">You clicked me {{ count }} times.</button>
</template>