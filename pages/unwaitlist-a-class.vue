<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Start Checking Your Course</h2>
        <br>
        <v-layout justify-center wrap xs12 md6 lg4>
            <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfwEiIB7jQnAqv9RcDmuLHoNMPsBiAHxI5b0sBW7uwmDL5p8g/viewform?embedded=true" width="640" height="766" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
        </v-layout>
      </div>
    </v-flex>
  </v-layout>
</template>

<style scoped>
/* PURCHASE RELATED STYLES ------------------------------------------------ */

/* package card styles */
.my-card {
  flex: 1 1 auto;
  margin: 10px;
  display: flex;
  flex-direction: column;
}

.my-card .my-card-title {
  font-weight: bold;
}


/* add/remove btn styles*/
.btn-wrapper {
  display: flex;
  justify-content: flex-end;
}


/* adds border movement to cards */
@media screen and (max-width: 960px) {
  .v-card.v-card.v-card {
    border-left: 3px solid #FFC107;
    border-top: none;
  }
}
</style>


<script>
export default {
  head() {
    return {
      title: 'Unwaitlist A Class'
    }
  }
}
</script>

