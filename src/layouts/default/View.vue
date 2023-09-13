<template>
  <v-layout>
      <v-main> 
        <v-container class="fill-height">
          <v-responsive class="d-flex align-center text-center fill-height">
            <router-view />
          </v-responsive>
        </v-container>
    </v-main>
  </v-layout>
</template>

<script setup>
import { ref } from 'vue'
const posts = ref([
  { value: 1, title: 'My journey with Vue', slug: 'slug1' },
  { value: 2, title: 'Blogging with Vue', slug: 'slug2' },
  { value: 3, title: 'Why Vue is so fun', slug: 'slug3' }
])

</script>
