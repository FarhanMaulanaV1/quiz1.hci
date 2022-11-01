<template>
  <ion-page>
    <ion-content>

      <ion-title>Home</ion-title>
      <ion-grid fixed>
        <ion-row class="statusrow">
          <ion-col size="6">
            <ion-card color ="dark">
              <ion-card-header>
                <ion-card-subtitle>Kolam</ion-card-subtitle>
                <ion-card-title>10</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col size="6">
            <ion-card color ="dark">
              <ion-card-header>
                <ion-card-subtitle>Kolam Aktif</ion-card-subtitle>
                <ion-card-title>8</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row class="statusrow">
          <ion-col size="6">
            <ion-card color= "dark">
              <ion-card-header>
                <ion-card-subtitle>Ikan Hidup</ion-card-subtitle>
                <ion-card-title>182 ekor</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col size="6">
            <ion-card color= "dark">
              <ion-card-header>
                <ion-card-subtitle>Ikan Mati</ion-card-subtitle>
                <ion-card-title>89 ekor</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
        <ion-row class="statusrow">
          <ion-col size="6">
            <ion-card color="dark">
              <ion-card-header>
                <ion-card-subtitle>Panen 2022</ion-card-subtitle>
                <ion-card-title>109 Kg</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
          <ion-col size="6">
            <ion-card color="dark">
              <ion-card-header>
                <ion-card-subtitle>Total Pakan</ion-card-subtitle>
                <ion-card-title>223 Kg</ion-card-title>
              </ion-card-header>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>

      <ion-title>Total Berat Ikan</ion-title>
      <swiper :slides-per-view="2" :loop="true">
        <swiper-slide>
          <ion-card color="dark" class="berat">
            <img src="assets/img/lele.png" alt="lele" class="ikan">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h3 class="judul">Lele</h3></ion-text></ion-card-title>
              <ion-text color="primary"><h4>200 Kg</h4></ion-text>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
        <swiper-slide>
          <ion-card color="dark" class="berat">
            <img src="assets/img/nila.png" alt="nila" class="ikan">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h3 class="judul">Nila</h3></ion-text></ion-card-title>
              <ion-text color="primary"><h4>200 Kg</h4></ion-text>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
        <swiper-slide>
          <ion-card color="dark" class="berat">
            <img src="assets/img/lele.png" alt="lele" class="ikan">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h3 class="judul">Lele</h3></ion-text></ion-card-title>
              <ion-text color="primary"><h4>200 Kg</h4></ion-text>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
        <swiper-slide>
          <ion-card color="dark" class="berat">
            <img src="assets/img/nila.png" alt="nila" class="ikan">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h3 class="judul">Nila</h3></ion-text></ion-card-title>
              <ion-text color="primary"><h4>200 Kg</h4></ion-text>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
      </swiper>

      <ion-title>Kualitas Air</ion-title>
      <swiper :slides-per-view="2" :loop="true">
        <swiper-slide>
          <ion-card color="dark" class="kualitas">
            <ion-card-header>
              <ion-card-title><ion-text color="light" ><h1 class="judul">pH</h1></ion-text></ion-card-title>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
        <swiper-slide>
          <ion-card color="dark" class="kualitas">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h1 class="judul">DO</h1></ion-text></ion-card-title>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
        <swiper-slide>
          <ion-card color="dark" class="kualitas">
            <ion-card-header>
              <ion-card-title><ion-text color="light"><h1 class="judul">Suhu</h1></ion-text></ion-card-title>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
              <ion-row>
                <ion-col size="6"></ion-col>
                <ion-col size="6"></ion-col>
              </ion-row>
            </ion-card-header>

            <ion-card-content>
            </ion-card-content>
          </ion-card>
        </swiper-slide>
      </swiper>
    </ion-content>

    <ion-footer :translucent="true">
      <ion-toolbar>
        <ion-title></ion-title>
      </ion-toolbar>
    </ion-footer>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonPage, IonTitle, IonGrid, IonCol, IonCard, IonToolbar, IonFooter,IonText} from '@ionic/vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
import { defineComponent } from 'vue';

import 'swiper/css';
import '@ionic/vue/css/ionic-swiper.css';

export default defineComponent({
  name: 'HomePage',
  components: {
    IonContent,
    IonPage,
    IonTitle,
    IonGrid,
    IonCol,
    IonCard,
    IonToolbar,
    IonFooter,
    Swiper,
    SwiperSlide,
    IonText
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
ion-title{
  margin-top: 10px;
}

#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}

ion-card{
  border-radius: 10px;
}
img.ikan{
  height: 150px;
  width: 200px;
}

ion-text .judul{
  text-align: left;
  font-weight: bold;
  margin-top: -10px;
}

ion-card.kualitas{
  width: 400px;
}
</style>
