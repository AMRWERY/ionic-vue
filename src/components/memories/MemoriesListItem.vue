<template>
  <ion-item :router-link="`/memories/${memory.id}`">
    <ion-thumbnail slot="start">
      <ion-img :src="memory.image"></ion-img>
    </ion-thumbnail>
    <ion-label>
      {{ memory.title }}
    </ion-label>
  </ion-item>
</template>

<script>
import { IonItem, IonImg, IonThumbnail, IonLabel } from "@ionic/vue";

export default {
  components: { IonItem, IonImg, IonThumbnail, IonLabel },

  props: ["memory"],
};
</script>
