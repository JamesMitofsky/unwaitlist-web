<template>
  <v-app dark>

    <div class="error-content">
<h1 v-if="error.statusCode === 404">
      {{ pageNotFound }}
    </h1>
    <h1 v-else>
      {{ otherError }}
    </h1>

    <div>Yikes, that was embarassing. We're sorry.</div>
    <br>
    <div>If we can help out, bop us on our <nuxt-link to="/contact">Contact</nuxt-link> page.</div>

    </div>
    
  </v-app>
</template>

<script>
export default {
  layout: 'empty',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  head() {
    const title =
      this.error.statusCode === 404 ? this.pageNotFound : this.otherError
    return {
      title
    }
  },
  data() {
    return {
      pageNotFound: '404 Not Found',
      otherError: 'An error occurred'
    }
  }
}
</script>

<style scoped>
.error-content {
  text-align: center;

}
</style>
