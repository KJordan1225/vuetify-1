<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>


<template>
  <v-app class="rounded rounded-md">
    <!-- <v-app-bar title="Application bar"> -->
      <v-toolbar density="compact">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>
          <RouterLink to="/">Annual Raffle</RouterLink>
        </v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn
          to="/buytickets"
          variant="outlined"
          size="small"
        >
          Buy Tickets
        </v-btn>

        <v-btn
          to="/learnmore"
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

    <!-- </v-app-bar> -->

    <!-- <v-navigation-drawer>
      <v-list>
        <v-list-item title="Navigation drawer"></v-list-item>
      </v-list>
    </v-navigation-drawer> -->

    <v-main style="min-height: 300px;">
      <!-- Main Content -->
      <RouterView />
    </v-main>
  </v-app>
</template>

