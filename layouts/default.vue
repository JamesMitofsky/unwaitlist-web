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
        <nuxt-link class="home-link" to="/">unwaitlist.io</nuxt-link>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn text href="#phil-header-container">Our Phil</v-btn>
        <v-btn text to="blank">Join the fam</v-btn>
        <v-btn text to="blank">Contact</v-btn>
      </v-toolbar-items>
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

/* import smiler font */
@font-face {
  font-family: 'Smiler';
  src: url(../assets/Smiler.ttf) format('truetype');
}
.home-link {
  font-family: 'Smiler';
}
</style>
