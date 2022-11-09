<template>
    
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-grid fixed>
                    <ion-row>
                        <ion-col size="1">
                            
                        </ion-col>
                        <ion-col size="11">
                            <ion-text color="dark" >
                            <h1 class="judul">Registrasi Kolam</h1>
                            </ion-text>
                        </ion-col>
                    </ion-row>
                </ion-grid>
            </ion-toolbar>
        </ion-header>
      <ion-content :fullscreen="true">
        <ion-list lines="none">
            <ion-item>
                <ion-label position="stacked">Nama Kolam</ion-label>
                <ion-textarea placeholder="Kolam 1"></ion-textarea>
            </ion-item>
            <ion-item>
                <ion-label position="stacked">Lokasi Kolam</ion-label>
                <ion-textarea placeholder="Block A"></ion-textarea>
            </ion-item>
            <ion-item>
                <ion-label>Material Kolam</ion-label>
                <ion-select interface="action-sheet">
              <ion-select-option value="tanah">Tanah</ion-select-option>
              <ion-select-option value="beton">Beton</ion-select-option>
              <ion-select-option value="terpal">Terpal</ion-select-option>
            </ion-select>
            </ion-item>
            <ion-item>
                <ion-label>Bentuk Kolam</ion-label>
                <ion-select interface="action-sheet">
              <ion-select-option value="tanah">Tanah</ion-select-option>
              <ion-select-option value="beton">Beton</ion-select-option>
              <ion-select-option value="terpal">Terpal</ion-select-option>
            </ion-select>
            </ion-item>
            <ion-item>
                <ion-button expand="block" color="tertiary">
                    <h3>Registrasi</h3>
                </ion-button>
            </ion-item>
        </ion-list>
      </ion-content>
  
    </ion-page>
</template>
  
  <script lang="ts">
  import { IonContent, IonPage, IonHeader, IonToolbar, IonGrid, IonCol, IonRow, IonList, IonItem, IonLabel, IonButton} from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  
  
  export default defineComponent({
    name: 'HomePage',
    components: {
      IonContent,
      IonPage,
      IonHeader,
      IonToolbar,
      IonGrid,
      IonCol,
      IonRow,
      IonList,
      IonItem,
      IonLabel,
      IonButton
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
  ion-text .judul{
    text-align: center;
  }
  ion-button{
    width: 100%;
    height: 50px;
  }
  </style>
  