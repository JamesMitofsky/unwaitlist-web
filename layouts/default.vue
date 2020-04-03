<template>
  <v-app>
    <v-app-bar color="#016030" app>
      <v-toolbar-title class="my-toolbar-title">
        <nuxt-link class="unwaitlist-logo-container smiler-font" to="/">
          <img class="logo" src="../static/icon.png" alt="Logo" />
          <span class="header-text-pronounced">unwaitlist</span>
          <span class="header-text-muted">.io</span>
        </nuxt-link>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="my-toolbar-items">
        <v-btn text to="/">
        <img class="nav-svg" src="../static/home.svg" alt="Graphic: Home">
        Our Phil</v-btn>
        <v-btn text to="/register">
        <img class="nav-svg" src="../static/clipboard.svg" alt="Graphic: Sign-up">
        Register</v-btn>
        <v-btn text to="/contact">
        
        <img class="nav-svg" src="../static/email.svg" alt="Graphic: Contact">
        Contact</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-content class="my-content">
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer class="footer" dark>
      <span>James Tedesco &copy; 2019</span>

      <v-spacer></v-spacer>
      <a target="_blank" href="https://github.com/JamesTedesco/unwaitlist.io" class="made-with-love">Made with ❤️ in BTV</a>
    </v-footer>
  </v-app>
</template>

<style scoped>
/* NAVBAR STYLES */

.v-toolbar__content.v-toolbar__content.v-toolbar__content {
  padding: 0;
}

.header-text-pronounced {
  color: white;
}

.header-text-muted {
  color: hsl(152, 39%, 72%);
}

.my-toolbar-title a {
  color: white;
  text-decoration: none;
}

.my-toolbar-items .v-btn {
  color: #d3eed9;
}

.nav-svg {
  height: 17px;
  margin: 0 6px;
}

/* Control logo size */
.unwaitlist-logo-container {
  display: flex;
  align-items: center;
}
.logo {
  width: 40px;
  margin-right: 5px;
  max-width: 44px;
}

/* move the injected content down */
.my-content {
  margin-top: 15px;
  background-color: white;
}

/* sets navbar text as dynamic when screen is small*/
@media screen and (max-width: 600px) {
  .my-toolbar-title {
    font-size: 3.3vw;
  }
  .my-toolbar-items .v-btn.v-btn {
    font-size: 12px;
    padding: 0 8px;
  }
  /* hide unwaitlist.io name when screen too small */
  .header-text-pronounced, .header-text-muted {
    display: none;
  }
}

@media screen and (max-width: 399px) {
  .logo {
    width: 5vw;
  }
}

/* import smiler font */
@font-face {
  font-family: 'Smiler';
  src: url(../assets/Smiler.ttf) format('truetype');
}
.smiler-font {
  font-family: 'Smiler';
}

/* FOOTER STYLES */
.v-footer .made-with-love {
  font-size: 10px;
  color: white;
  text-decoration: none;
}

.v-footer.footer {
  background-color: #016030;
}

</style>


<script>
export default {
  head() {
    return {
      meta: [
        
        { name: 'apple-mobile-web-app-status-bar-style', content: 'default' },
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { charset: 'UTF-8' },
        // General SEO
        {
          name: 'description',
          content:
            'UVM students, get notified when your class has availability.'
        },
        {
          name: 'image',
          content: 'https://unwaitlist.io/unwaitlist-preview.png'
        },
        // Google
        { itemprop: 'name', content: 'unwaitlist' },
        {
          itemprop: 'description',
          content:
            'UVM students, get notified when your class has availability.'
        },
        {
          itemprop: 'image',
          content: 'https://unwaitlist.io/unwaitlist-preview.png'
        },
        // Twitter
        { name: 'twitter:card', content: 'summary' },
        { name: 'twitter:title', content: 'unwaitlist' },
        {
          name: 'twitter:description',
          content:
            'UVM students, get notified when your class has availability.'
        },
        {
          name: 'twitter:image:src',
          content: 'https://unwaitlist.io/unwaitlist-preview.png'
        },
        // Open Graph general (Facebook, Pintrest, & Google)
        { name: 'og:title', property: 'og:title', content: 'unwaitlist' },
        {
          name: 'og:description',  property: 'og:description',
          content:
            'UVM students, get notified when your class has availability.'
        },
        { name: 'og:image', property: 'og:image', content:'https://unwaitlist.io/unwaitlist-preview.png' },
        { name: 'og:url', property: 'og:url', content: 'https://unwaitlist.io/' },
        { name: 'og:site_name', property: 'og:site_name', content: 'unwaitlist' },
        { name: 'og:type',  property: 'og:type', content: 'product' }
      ]
    }
  }
}
</script>


