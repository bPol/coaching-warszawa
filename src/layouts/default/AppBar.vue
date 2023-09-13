<template>
        <v-app-bar
          app
          color="primary"
          dark
          flat
          >
            <v-app-bar-nav-icon />
        </v-app-bar>


        <v-navigation-drawer
            permanent
            location="right"
        >
            <v-list :items="posts">
            </v-list>
        </v-navigation-drawer>       
</template>

<script setup>
import posts from '@/data/posts.json'

</script>
