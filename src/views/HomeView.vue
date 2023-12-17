<template>
  <v-carousel 
    :show-arrows="false"
    cycle
    height="400"
    hide-delimiter-background
    show-arrows="hover"
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      cover
    >     
      <div class="d-flex fill-height justify-center align-center">
        <div class="text-h2 text-white" >
          {{ item.slides }} Prize: {{ item.prizes }}          
        </div>
      </div>
    </v-carousel-item>
</v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
            slides: 'First',
            prizes: '$2000',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
            slides: 'Second',
            prizes: '$1000',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
            slides: 'Third',
            prizes: '$500',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
            slides: 'Fourth',
            prizes: '50" Smart TV',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
            slides: 'Fifth',
            prizes: '$100',
          },
        ],
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
        prizes: [
          '$2000',
          '$1500',
          '$1000',
          '50 in nFlat-screen TV',
          '$100',
        ],
      }
    },
  }
</script>





