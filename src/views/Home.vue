<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Lista de Contatos</ion-title>
      </ion-toolbar>
    </ion-header>
    
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Lista de Contatos com Vuex</ion-title>
        </ion-toolbar>
      </ion-header>
    
      <div id="container">
        <ion-button expand="block" router-link="/chamada">Chamada à API</ion-button>
        <ion-button expand="block" router-link="/contatos">Exibe lista de contatos</ion-button>
      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonButton } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    IonButton
  }
});
</script>

<style scoped>
#container {
  text-align: center;
 
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

ion-button {
  margin: 20px
}
</style>