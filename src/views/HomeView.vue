<template>

<div class="text-h1 text-red">
  <center>WIN $2000!</center>
  <center>RAFFLE DRAWING</center>
  <center>MARCH 15</center>
</div>



<v-container class="bg-surface-variant">
    <v-row no-gutters>
      <v-col>
        <v-sheet class="pa-2 ma-2">


        <div>
          <section>
            <iframe width="500" height="400" src="https://www.youtube.com/embed/f-yh37DM7Dw?si=BPY0aoXEiEcOYSbh?autoplay=1" 
              title="YouTube video player" 
              frameborder="0" 
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
              allowfullscreen>
            </iframe>
          </section>
        </div>



        </v-sheet>
      </v-col>
      <v-col>
        <v-sheet class="pa-2 ma-2">
          

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



        </v-sheet>
      </v-col>
    </v-row>
  </v-container> 
  
  <br>
  <br>

  <div class="text-h1 text-red">
  <center>TICKETS ON SALE NOW!</center>
  <center>$20 EACH</center>
  </div>

  <br>

  <center>
    <v-btn 
      to="/buytickets"
      color="red"
      size="x-large"
    >
      Buy Tickets
    </v-btn>
  </center>
  

  <br>

  <!-- CONTENT V-CARD -->
  <br>
  <br>
  <div style="width:800px; margin:0 auto;">
  
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
      <v-btn 
        to="/buytickets"
        color="orange">
        Buy Tickets
      </v-btn>

      <v-btn 
        to="/learnmore"
        color="orange">
        Learn More
      </v-btn>
    </v-card-actions>
  </v-card>
  </div>

  
  <!-- https://youtu.be/f-yh37DM7Dw -->
  
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





