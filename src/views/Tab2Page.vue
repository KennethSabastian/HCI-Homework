<template>
  <ion-page>    
    <ion-content :fullscreen="true">
      <ion-item class="item1">
        <ion-label color="light" class="text1">
          Kolam
        </ion-label>
        <ion-icon :icon="list" slot="end" class="icon1"></ion-icon>
        <ion-icon :icon="funnel" slot="end" class="icon1"></ion-icon>
      </ion-item>
    <ion-card class="card1" color="light">
      <ion-item class="item1" color="light">
        <ion-label>
          Alpha
        </ion-label>
        <ion-button slot="end" color="success">aktif</ion-button>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarClear" slot="start"></ion-icon>
        <ion-label>01-09-2022</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarNumber" slot="start"></ion-icon>
        <ion-label>90 hari</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="fish" slot="start"></ion-icon>
        <ion-label>200 ekor</ion-label>
      </ion-item>
    </ion-card>
    <ion-card class="card1" color="light">
      <ion-item class="item1" color="light">
        <ion-label>
          Beta
        </ion-label>
        <ion-button slot="end" color="danger">tidak aktif</ion-button>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarClear" slot="start"></ion-icon>
        <ion-label>01-09-2022</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarNumber" slot="start"></ion-icon>
        <ion-label>90 hari</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="fish" slot="start"></ion-icon>
        <ion-label>200 ekor</ion-label>
      </ion-item>
    </ion-card>
    <ion-card class="card1" color="light">
      <ion-item class="item1" color="light">
        <ion-label>
          Charlie
        </ion-label>
        <ion-button slot="end" color="success">aktif</ion-button>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarClear" slot="start"></ion-icon>
        <ion-label>01-09-2022</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarNumber" slot="start"></ion-icon>
        <ion-label>90 hari</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="fish" slot="start"></ion-icon>
        <ion-label>200 ekor</ion-label>
      </ion-item>
    </ion-card>
    <ion-card class="card1" color="light">
      <ion-item class="item1" color="light">
        <ion-label>
          Delta
        </ion-label>
        <ion-button slot="end" color="success">aktif</ion-button>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarClear" slot="start"></ion-icon>
        <ion-label>01-09-2022</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarNumber" slot="start"></ion-icon>
        <ion-label>90 hari</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="fish" slot="start"></ion-icon>
        <ion-label>200 ekor</ion-label>
      </ion-item>
    </ion-card>
    <ion-card class="card1" color="light">
      <ion-item class="item1" color="light">
        <ion-label>
          Epsilon
        </ion-label>
        <ion-button slot="end" color="success">aktif</ion-button>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarClear" slot="start"></ion-icon>
        <ion-label>01-09-2022</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="calendarNumber" slot="start"></ion-icon>
        <ion-label>90 hari</ion-label>
      </ion-item>
      <ion-item lines="none" class="item2" color="light">
        <ion-icon :icon="fish" slot="start"></ion-icon>
        <ion-label>200 ekor</ion-label>
      </ion-item>
    </ion-card>
    </ion-content>
    <ion-fab vertical="bottom" horizontal="end">
      <ion-fab-button>
        <ion-icon :icon="add"></ion-icon>
      </ion-fab-button>
    </ion-fab>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonContent,IonItem,IonLabel, IonIcon, IonButton, IonCard,IonFab,IonFabButton } from '@ionic/vue';
import { funnel,list,calendarClear,calendarNumber, fish, add } from 'ionicons/icons';

export default defineComponent({
  name: 'Tab2Page',
  components: {  IonContent, IonPage, IonLabel,IonItem, IonIcon, IonButton,IonCard,IonFab,IonFabButton },
  setup() {
    return {
      funnel,
      list,
      calendarClear,
      calendarNumber,
      fish,
      add
    }
  }
});
</script>
  <style scoped>
  .card1{
    padding-top: 10px;
    padding-left: 10px;
    padding-right: 10px;
    margin-left: 40px;
    margin-right:40px;
    margin-top: 20px
  }
  .item1{
    font-size: 18px;
    font-weight: bold;
  }
  .item2{
    color:black;
    font-size: 16px;
    font-weight: 50;
  }
  .text1{
    font-size: 30px;
    font-weight: bold;
  }
  .icon1{
    color: white
  }
  </style>