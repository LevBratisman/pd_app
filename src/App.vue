<template>
  <v-app>
    <!-- App toolbar -->
    <v-app-bar elevation="12" rounded>

      <v-app-bar-title>{{ toolbar_title }}</v-app-bar-title>

    </v-app-bar>

    <v-dialog
      v-model="dialog"
      width="auto"
    >
      <v-card style="padding: 20px; border-radius: 20px;" variant="flat" color="dark-indigo" class="Mascot-wrapper">
        <v-card-text class="mascot">
          <h2>Добро пожаловать в SIMPLE PHYSICS!</h2>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="/Mascot.png"
          ></v-img>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <!-- <a href="#path" style="color: black; text-decoration: none;">
            <v-btn
            variant="elevated"
            color="green"
            @click="aboutUs"><a href="#path" style="color: black; text-decoration: none;">О нас</a>
            </v-btn>
          </a> -->
          <v-btn variant="elevated" color="gray" @click="this.dialog = false">Закрыть</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>

    <v-main style="padding-top: 0;">
      <RouterView />
    </v-main>

    <div id="path"></div>
  </v-app>
  
</template>

<script>
import { RouterView } from 'vue-router'
export default {
  data() {
    return {
      value: 1,
      toolbar_title: 'SIMPLE PHYSICS',
      dialog: true
    }
  },
  methods: {
    changeToolbarTitle(current_title) {
      this.toolbar_title = current_title;
    }
  }
}
</script>

<style>
.v-timeline-item__body {
  max-width: 400px;
}


.mascot {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>