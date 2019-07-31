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

      <v-toolbar-title class="toolbar-title ml-5">
        <nuxt-link to="/">unwaitlist.io</nuxt-link>
      </v-toolbar-title>
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
    return {}
  }
}
</script>

<style>
.toolbar-title a {
  color: black;
  text-decoration: none;
}
.toolbar-title a:hover {
  text-decoration: underline;
}
</style>
