<template>
  <ion-page>
    <ion-grid>
      <h1>Home</h1>
      <ion-row>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Kolam</ion-card-title>
              <ion-card-subtitle>10</ion-card-subtitle>
            </ion-card-header>


          </ion-card>
        </ion-col>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Kolam Aktif</ion-card-title>
              <ion-card-subtitle>8</ion-card-subtitle>
            </ion-card-header>


          </ion-card>
        </ion-col>
      </ion-row>
      <ion-row>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Ikan Hidup</ion-card-title>
              <ion-card-subtitle>182 Ekor</ion-card-subtitle>
            </ion-card-header>


          </ion-card>
        </ion-col>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Ikan Mati</ion-card-title>
              <ion-card-subtitle>89 Ekor</ion-card-subtitle>
            </ion-card-header>


          </ion-card>
        </ion-col>
      </ion-row>

      <ion-row>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Panen 2022</ion-card-title>
              <ion-card-subtitle>109 Kg</ion-card-subtitle>
            </ion-card-header>


          </ion-card>
        </ion-col>
        <ion-col>
          <ion-card>
            <ion-card-header>
              <ion-card-title>Total Pakan</ion-card-title>
              <ion-card-subtitle>223 Kg</ion-card-subtitle>
            </ion-card-header>
          </ion-card>
        </ion-col>
      </ion-row>

      <h1>Total Berat Ikan</h1>

      <ion-row>

        <h1>
          <ion-card>
            <center>
              <img alt="Lele"
                src="https://w7.pngwing.com/pngs/77/215/png-transparent-wels-catfish-oily-fish-carp-hazard-graphe-animals-photography-fauna-thumbnail.png" />
            </center>
            <ion-card-header>
              <head-title>Lele</head-title>
              <ion-card-title>
                <blue>200kg</blue>
              </ion-card-title>
            </ion-card-header>
          </ion-card>
        </h1>

        <h1>
          <ion-card>
            <center>
              <img alt="Nila Merah" src="https://efishery.com/wp-content/uploads/2022/05/ikan-nila-nifi.png" />
            </center>

            <ion-card-header>
              <head-title>Nila Merah</head-title>
              <ion-card-title>
                <blue>200kg</blue>
              </ion-card-title>
            </ion-card-header>
          </ion-card>
        </h1>
      </ion-row>


      <h1>Kualitas Air</h1>

      <ion-row>

        <h1>
          <ion-card>
            <ion-card-header>
              <h2>pH</h2>
              <br>
              <subtitle>Normal <blue>6 Kolam</blue>
              </subtitle><br>
              <subtitle>Abnormal <blue>6 Kolam</blue>
              </subtitle>

            </ion-card-header>
          </ion-card>
        </h1>

        <h1>
          <ion-card>
            <ion-card-header>
              <h2>DO</h2>
              <br>
              <subtitle>Normal <blue> 6 Kolam</blue>
              </subtitle><br>
              <subtitle>Abnormal <blue> 6 Kolam</blue>
              </subtitle>

            </ion-card-header>
          </ion-card>
        </h1>


      </ion-row>

    </ion-grid>
  </ion-page>
</template>

<script lang="ts">
import { IonCol, IonGrid, IonRow } from '@ionic/vue';
import { IonCard, IonCardHeader, IonCardSubtitle, IonCardTitle, IonPage } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomePage',
  components: { IonCol, IonGrid, IonRow, IonCard, IonCardHeader, IonPage, IonCardSubtitle, IonCardTitle, },
  setup() {
    const slideOpts = {
      initialSlide: 2,
      speed: 400
    };
    return { slideOpts }
  }
});
</script>

<style scoped>
body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: white;
}

h1 {
  font-size: 20px;
  font-weight: 600;
  margin-left: 10px;
}

ion-card-title {
  font-size: 20px;
  color: black;
  font-weight: 700;
}

ion-card-subtitle {
  font-size: 25px;
  font-weight: 600;

  /* margin-top: 10px; */
  text-transform: capitalize;
  color: black;
}

subtitle {
  font-size: 15px;
  font-weight: 600;

  /* margin-top: 10px; */
  text-transform: capitalize;
  color: black;
}

ion-card {
  background-color: aliceblue;
  /* height: 100px; */
  padding: 0;
  margin: 2px;

}

img {
  margin: auto;
  padding: 10px;
  height: 150px;
  width: 180px;
}

h2 {
  font-size: 30px;
  color: black;
  margin: 0;
  font-weight: 600;
}

blue {
  color: #2C96F1;
  font-weight: bold;
}

head-title {
  margin-top: 0;
  font-size: 20px;
  color: black;
}


/* ion-col {
      background-color: #135d54;
      border: solid 1px #fff;
      color: #fff;
      text-align: center;
    } */
</style>
