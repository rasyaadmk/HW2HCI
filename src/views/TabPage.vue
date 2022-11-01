<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="HomePage" href="/tabs/home">
          <ion-icon name="home-outline"></ion-icon>
        </ion-tab-button>

        <ion-tab-button tab="PageSecond" href="/tabs/Page2">
          <ion-icon src="/assets/icon/page2.svg" />
        </ion-tab-button>

      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue';
import { IonTabBar, IonTabButton, IonTabs, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { ellipse, triangle } from 'ionicons/icons';

export default defineComponent({
  name: 'TabsPage',
  components: { IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage, IonRouterOutlet },
  setup() {
    return {
      ellipse,
      triangle,
    }
  }
});
</script>

<style scoped>
ion-tab-bar {
  background-color: #252836;
  border-radius: 15px 15px 0px 0px;
}

ion-tab-button {
  background-color: #252836;
}
</style>
  