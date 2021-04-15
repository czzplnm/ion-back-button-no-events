<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-button @click="() => router.push('/tabs/tab1')">Go to tabs</ion-button>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
  import {IonPage, IonHeader, IonToolbar, IonTitle, IonContent} from '@ionic/vue';

  import {useRouter} from 'vue-router';

  export default {
    name: 'Tab1',
    components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage},
    setup() {
      const router = useRouter();
      return {router};
    },
  }
</script>