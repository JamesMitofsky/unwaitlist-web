<template>
  <v-app>
    <v-app-bar class="nav-bar" app>
      <v-toolbar-title class="my-toolbar-title">
        <nuxt-link class="home-link" to="/">
          <span class="header-text-pronounced">unwaitlist</span>
          <span class="header-text-muted">.io</span>
        </nuxt-link>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="my-toolbar-items">
        <v-btn text to="/">Our Phil</v-btn>
        <v-btn text to="/packages">Packages</v-btn>
        <v-btn text to="/contact">Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <v-content class="my-content">
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer dark>
      <span>James Tedesco &copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  head () {
    return {
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {charset: "UTF-8"},
        // General SEO
        {name:"description", content: "A service designed to help get University of Vermont students off the course waitlist."},
        {name:"image", content:"https://unwaitlist.io/unwaitlist-preview.png"},
        // Google
        {itemprop:"name", content:"unwaitlist"},
        {itemprop:"description", content:"A service designed to help get University of Vermont students off the course waitlist."},
        {itemprop:"image", content:"https://unwaitlist.io/unwaitlist-preview.png"},
        // Twitter
        {name:"twitter:card", content:"summary"},
        {name:"twitter:title", content:"unwaitlist"},
        {name:"twitter:description", content:"A service designed to help get University of Vermont students off the course waitlist."},
        {name:"twitter:image:src", content:"https://unwaitlist.io/unwaitlist-preview.png"},
        // Open Graph general (Facebook, Pintrest, & Google)
        {name:"og:title", content:"unwaitlist"},
        {name:"og:description", content:"A service designed to help get University of Vermont students off the course waitlist."},
        {name:"og:url", content:"https://unwaitlist.io/"},
        {name:"og:site_name", content:"unwaitlist"},
        {name:"og:type", content:"product"}
      ]
    }
  }
}

</script>

<style>
/* NAVBAR STYLES */
.v-app-bar.nav-bar {
  background-color: #2c769b;
}

.header-text-pronounced {
  color: hsla(200, 66%, 94%, 1);
}

.header-text-muted {
  color: hsla(200, 51%, 67%, 1);
}

.my-toolbar-title a {
  color: hsla(200, 66%, 94%, 1);
  text-decoration: none;
}

.my-toolbar-items .v-btn {
  color: #d3e5ee;
}

/* move the injected content down */
.my-content {
  margin-top: 15px;
}

/* sets navbar text as dynamic when screen is small*/
@media screen and (max-width: 600px) {
  .my-toolbar-title {
    font-size: 3.3vw;
  }
  .my-toolbar-items .v-btn.v-btn {
    font-size: 3.2vw;
    padding: 0 8px;
  }
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
