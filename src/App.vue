<template>
  <v-app>
    <v-app-bar
      app
      color="secondary"
      dark
    >
      <div class="d-flex align-center">
        <h1>Avi Dalal</h1>
      </div>

      <v-spacer></v-spacer>


    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
    <v-footer
        dark
        padless
    >
      <v-card
          class="flex"
          flat
          tile
      >

        <v-card-text class="py-2 white--text text-center">
          {{ new Date().getFullYear() }} — <strong>Avi Dalal</strong>
        </v-card-text>
      </v-card>
    </v-footer>

  </v-app>


</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
//
  }),
};
</script>
