<template>
  <v-app>
    <v-main>
      <v-app-bar app color="primary" dark>
        <v-toolbar-title>Most Used Words In Captions</v-toolbar-title>
      </v-app-bar>

      <v-container>
        <home />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Home from './components/HomeComponent.vue'
export default {
  name: 'App',

  components: {
    Home
  },

  data: () => ({
    //
  }),
}
</script>
