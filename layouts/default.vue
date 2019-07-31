<template>
  <v-app>
    <v-app-bar app>
      <v-img
        class="mx-2"
        :src="require('~/assets/number.png')"
        max-height="50"
        max-width="50"
        contain
      ></v-img>

      <v-toolbar-title class="ml-5" v-text="title" />
    </v-app-bar>

    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer dark>
      <span>&copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: 'unwaitlist.io'
    }
  }
}
</script>
