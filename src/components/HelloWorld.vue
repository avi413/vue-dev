<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/ad.webp')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          This is my Welcome
        </h1>

        <p class="subheading font-weight-regular">
          my Desc
          <br>new line Desc

        </p>
      </v-col>



      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Important Links
        </h2>

        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            <i :class="link.fw+' fa-'+link.text"></i>
          </a>
        </v-row>
      </v-col>


    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({

      importantLinks: [
        {
          fw: 'fa',
          text: 'address-card',
          href: 'https://avidalal.net',
        },
        {
          fw: 'fab',
          text: 'facebook',
          href: 'https://community.vuetifyjs.com',
        },
        {
          fw: 'fab',
          text: 'twitter',
          href: 'https://madewithvuejs.com/vuetify',
        },

      ],

    }),
  }
</script>
