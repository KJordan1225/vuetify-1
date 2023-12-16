<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <!-- <v-card
    color="grey-darken-4"
    flat
    height="200px"
    rounded="0"
  > -->
    <v-toolbar density="compact">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Annual Raffle</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn
        variant="outlined"
        size="small"
      >
        Buy Tickets
      </v-btn>

      <v-btn
        variant="outlined"
        size="small"
      >
        Learn More
      </v-btn>

      <!-- <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn> -->
    </v-toolbar>
  <!-- </v-card> -->
</template>
