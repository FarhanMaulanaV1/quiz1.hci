<template>
    <ion-page>
      <ion-content>
        <h1>oke udah</h1>
      </ion-content>
  
    </ion-page>
  </template>
  
  <script lang="ts">
  import { IonContent, IonPage} from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  
  
  export default defineComponent({
    name: 'HomePage',
    components: {
      IonContent,
      IonPage,
    },
    setup() {
      // Optional parameters to pass to the swiper instance. See https://swiperjs.com/swiper-api for valid options.
      const slideOpts = {
        initialSlide: 1,
        speed: 400
      };
      return { slideOpts }
    }
  
  });
  
  
  </script>
  
  <style scoped>

  </style>
  