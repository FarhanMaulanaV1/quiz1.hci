<template>
    
    <ion-page>
        <ion-header :translucent="true">
            <ion-toolbar>
                <ion-grid>
                <ion-row>
                    <ion-col>
                    <ion-title class="ion-float-left">Kolam</ion-title>
                    </ion-col>
                    <ion-col size="1">
                    <ion-icon src="assets/img/Sorting.svg"></ion-icon>
                    </ion-col>
                    <ion-col size="1.1">
                    <ion-icon src="assets/img/Vector.svg"></ion-icon>
                    </ion-col>
                </ion-row>
                </ion-grid>
            </ion-toolbar>
        </ion-header>
      <ion-content :fullscreen="true">
        <ion-list lines="none">
            <ion-item>
                <ion-card color="dark"  v-for="(pond,index) in pondDetails" v-bind:key="index">
                    <ion-item lines="inset" color="dark">
                    <ion-label><strong>{{pondDetails.alias}}</strong></ion-label>
                    <ion-button slot="end" size="small" color="success">
                        {{pondDetails.status}}
                    </ion-button>
                    </ion-item>
                    <ion-card-content>
                    <ion-grid>
                        <ion-row class="ion-justify-content-start">
                        <ion-col size="1"
                            ><ion-icon src="assets/img/calendar+.svg"></ion-icon
                        ></ion-col>
                        <ion-col size="auto"><p>{{pondDetails.build_at}}</p></ion-col>
                        </ion-row>
                        <ion-row class="ion-justify-content-start">
                        <ion-col size="1"
                            ><ion-icon src="assets/img/calendar.svg"></ion-icon
                        ></ion-col>
                        <ion-col size="auto"><p>90 hari</p></ion-col>
                        </ion-row>
                        <ion-row class="ion-justify-content-start">
                        <ion-col size="1"
                            ><ion-icon src="assets/img/fish.svg"></ion-icon
                        ></ion-col>
                        <ion-col size="auto"><p>{{pondDetails.fish_alive}}</p></ion-col>
                        </ion-row>
                    </ion-grid>
                    </ion-card-content>
                </ion-card>
            </ion-item>
        </ion-list>
        <ion-fab vertical="bottom" horizontal="end" slot="fixed">
            <ion-fab-button color="tertiary" href="/register">
            <ion-icon src="assets/img/tandatambah.svg"></ion-icon>
            </ion-fab-button>
        </ion-fab>
      </ion-content>
  
    </ion-page>
</template>
  
  <script lang="ts">
  import { IonContent, IonPage, IonIcon,IonHeader,IonToolbar,IonGrid,IonRow,IonCol, IonList, IonItem,IonFab,IonFabButton, IonButton} from '@ionic/vue';
  import { defineComponent, onMounted, ref } from 'vue';
  import axios from 'axios';
  
  
  
  export default defineComponent({
    name: 'HomePage',
    components: {
      IonContent,
      IonPage,
      IonIcon,
      IonHeader,
      IonToolbar,
      IonGrid,
      IonRow,
      IonCol,
      IonList,
      IonItem,
      IonFab,
      IonFabButton,
      IonButton
    },
    setup() {
      const pondDetails = ref();
      onMounted(async() => {
            const response = await axios.get('http://jft.web.id/fishapi/api/ponds');
            pondDetails.value = response.data;
            console.log(response.data);
      });
      return{
        pondDetails
      };
    }
  
  });
  
  
  </script>
  
  <style scoped>
  ion-card{
    border-radius: 20px;
    width: 100%;
  }

  </style>
  