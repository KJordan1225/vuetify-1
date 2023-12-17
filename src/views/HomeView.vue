<template>
  <v-carousel 
    :show-arrows="true"
    cycle
    height="400"
    hide-delimiter-background
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.source"
      cover
    >     
      <div class="d-flex fill-height justify-center align-center">
        <div class="text-h1 text-white" >
          {{ item.slides }} Prize: {{ item.prizes }}          
        </div>
      </div>
    </v-carousel-item>
  </v-carousel>

  <!-- CONTENT V-CARD -->
  <br>
  <br>

  <v-card
    class="mx-auto"
    max-width="800"
  >
    <v-img
      class="align-end text-white"
      height="200"
      src="http://localhost:5173/images/carousel/HANDING-CASH.jpg"
      cover
    >
      <v-card-title>Gamma Alpha Annual Raffle - TICKETS ON SALE NOW !!!</v-card-title>
    </v-img>

    <v-card-subtitle class="pt-4 text-bold">
      Benefitting Our Scholarship and Socual Action Programs
    </v-card-subtitle>

    <v-card-text>
      
        <div>Prizes:</div>
        <br>
        <div>
          <ul>
            <li>FIRST PLACE:   $2000</li>
            <li>SECOND PLACE:  $1000</li>
            <li>THIRD PLACE:   $500</li>
            <li>FOUTH PLACE:   50" Smart TV</li>
            <li>FIFTH PLACE:   $100</li>
          </ul>
        </div>
        <br>
        <div>Drawing:  March 15</div>
        <div>Tickets: $20 ea.</div>
        <div>Credit/Debit cards ACCEPTED</div>
        <div>Winners DO NOT need to be present to win.</div>
          
    </v-card-text>

    <v-card-actions>
      <v-btn color="orange">
        Buy Tickets
      </v-btn>

      <v-btn color="orange">
        Learn More
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script setup lang="ts">
  
  import { ref } from 'vue'

  const items = ref([
    {source: 'http://localhost:5173/images/carousel/CASH-4.jpg',
     slides: 'First',
     prizes: '$2000'},
    {source: 'http://localhost:5173/images/carousel/CASH-5.jpg',
     slides: 'Second',
     prizes: '$1000'},
    {source: 'http://localhost:5173/images/carousel/CASH-1A.jpg',
     slides: 'Third',
     prizes: '$500'},
    {source: 'http://localhost:5173/images/carousel/2000USD-1.jpg',
     slides: 'Fourth',
     prizes: '50" Smart TV'},
    {source: 'http://localhost:5173/images/carousel/HANDING-CASH.jpg',
     slides: 'Fifth',
     prizes: '$100'},
  ])


</script>





