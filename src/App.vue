<template>
  <v-app>
    <!-- App toolbar -->
    <v-app-bar elevation="12" rounded>

      <v-app-bar-title>{{ toolbar_title }}</v-app-bar-title>

    </v-app-bar>

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