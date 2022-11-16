<template>
  <ion-page>

    <ion-content :fullscreen="true">
      <div class="kolam-header" style="margin-inline: 30px;">
        <h1>Kolam</h1>
        <div>
          <img class="sort-icon" src="/assets/page2/sorting.svg" alt="">
          <img src="/assets/page2/sort.svg" alt="">
        </div>
      </div>
      <div>
        <ion-card class="box">
          <ion-card-header>
            <div class="cardhead" style="display: flex; justify-content: space-between;">
              <ion-card-title style="color: black; margin-top: 12px;">Alpha</ion-card-title>
              <button class="actv">Aktif</button>
            </div>
            <hr>
          </ion-card-header>

          <ion-card-content>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Calendar Plus.svg">
              <p>01-09-2022</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Timesheet.svg">
              <p>90 Hari</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Whole Fish.svg">
              <p>200 Ekor</p>
            </div>
          </ion-card-content>
        </ion-card>

        <ion-card class="box">
          <ion-card-header>
            <div class="cardhead" style="display: flex; justify-content: space-between;">
              <ion-card-title style="color: black; margin-top: 12px;">Beta</ion-card-title>
              <button class="actv">Aktif</button>
            </div>
            <hr>
          </ion-card-header>

          <ion-card-content>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Calendar Plus.svg">
              <p>01-09-2022</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Timesheet.svg">
              <p>90 Hari</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Whole Fish.svg">
              <p>200 Ekor</p>
            </div>
          </ion-card-content>
        </ion-card>
        <ion-card class="box">
          <ion-card-header>
            <div class="cardhead" style="display: flex; justify-content: space-between;">
              <ion-card-title style="color: black; margin-top: 12px;">Charlie</ion-card-title>
              <button class="actv">Aktif</button>
            </div>
            <hr>
          </ion-card-header>

          <ion-card-content>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Calendar Plus.svg">
              <p>01-09-2022</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Timesheet.svg">
              <p>90 Hari</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Whole Fish.svg">
              <p>200 Ekor</p>
            </div>
          </ion-card-content>
        </ion-card>
        <ion-card class="box">
          <ion-card-header>
            <div class="cardhead" style="display: flex; justify-content: space-between;">
              <ion-card-title style="color: black; margin-top: 12px;">Delta</ion-card-title>
              <button class="non-active">Tidak Aktif</button>
            </div>
            <hr>
          </ion-card-header>

          <ion-card-content>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Calendar Plus.svg">
              <p>01-09-2022</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Timesheet.svg">
              <p>90 Hari</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Whole Fish.svg">
              <p>200 Ekor</p>
            </div>
          </ion-card-content>
        </ion-card>
        <ion-card class="box">
          <ion-card-header>
            <div class="cardhead" style="display: flex; justify-content: space-between;">
              <ion-card-title style="color: black; margin-top: 12px;">Epsilon</ion-card-title>
              <button class="actv">Aktif</button>
            </div>
            <hr>
          </ion-card-header>

          <ion-card-content>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Calendar Plus.svg">
              <p>01-09-2022</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Timesheet.svg">
              <p>90 Hari</p>
            </div>
            <div class="hari" style="display: flex; gap: 10px; align-items: center;">
              <img src="/assets/page2/Whole Fish.svg">
              <p>200 Ekor</p>
            </div>
          </ion-card-content>
        </ion-card>
      </div>
    </ion-content>
    <ion-fab vertical="bottom" horizontal="end" slot="fixed">
      <ion-fab-button href="/registrationpage"><span style="font-size: 60px; font-weight:bolder">+</span>
      </ion-fab-button>
    </ion-fab>
  </ion-page>

</template>
  
<script lang="ts">
import { IonContent, IonPage } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageSecond',
  components: {
    IonContent,
    IonPage
  }
});
</script>
  
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

* {
  font-family: Poppins, sans-serif;
}

.kolam-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 15px 12px;
  font-weight: bold;
}

.kolam-header img {
  width: 30px;
}


hr {
  border-top: 2px solid black;
  margin-bottom: -10px;
}

ion-card-title {
  font-weight: 600;
}

.non-active {
  margin-top: 10px;
  margin-left: 180px;
  justify-content: center;
  align-items: center;
  padding: 5px 10px;
  gap: 10px;
  font-weight: 600;
  width: 100px;
  height: 34px;

  background: #c20000;
  border-radius: 12px;
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

.sort-icon {
  margin-right: 20px;
}

.box {
  padding: 1px 0px;
  font-family: poppin;
  background-color: white;
  color: black;
  margin: 15px 30px;
  border-radius: 16px;
  font-size: 18px;
  font-weight: 600;
  line-height: 27px;
}

.cardhead {
  columns: 2;
  margin-block: -5px, 10px;
}

.actv {
  margin-top: 10px;
  margin-left: 180px;
  justify-content: center;
  align-items: center;
  padding: 5px 10px;
  gap: 10px;
  letter-spacing: 0.05em;
  font-weight: 600;
  width: 58px;
  height: 34px;

  background: #1B7C1A;
  border-radius: 12px;
}
</style>
  