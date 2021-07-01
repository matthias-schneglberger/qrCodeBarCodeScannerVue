<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >

      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <v-container>
        <v-row>
          <v-col class="d-flex justify-center">
            <QrCodeComponent style="height: 500px; width: 500px"/>
          </v-col>
          <v-col class="d-flex justify-center">
            <BarcodeComponent style="height: 1000px; width: 800px"/>
          </v-col>
        </v-row>
      </v-container>

    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
// import HelloWorld from './components/HelloWorld.vue'
import QrCodeComponent from './components/QrCodeComponent.vue'
import BarcodeComponent from './components/BarcodeComponent.vue'

export default Vue.extend({
  name: 'App',

  components: {
    QrCodeComponent,
    BarcodeComponent
  },

  data: () => ({
    //
  })
})
</script>
