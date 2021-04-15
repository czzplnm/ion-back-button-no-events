<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button default-href="/installations"></ion-back-button>
          <ion-menu-button></ion-menu-button>
        </ion-buttons>
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
  import {
    IonPage,
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonBackButton,
    IonButtons,
    IonMenuButton
  } from '@ionic/vue';

  export default {
    name: 'Tab1',
    components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonBackButton, IonButtons, IonMenuButton},

    ionViewWillLeave() {
      console.log('ionViewWillLeave');
    },

    ionViewDidLeave() {
      console.log('ionViewDidLeave');
    },

    ionViewDidEnter() {
      console.log('ionViewDidEnter');
    },
  }
</script>