<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h1 class="fun-headers">Join the Fam</h1>
        <p>
          You're barely treading water and we definitely saw your head bob under. Thank goodness this program is better at
          unwaitlisting people than Zac Efron is at pretending to be a life guard.
        </p>
        <v-layout justify-center wrap xs12 md6 lg4>
            <v-card class="my-card">
              <v-card-title class="my-card-title">✅ Unwaitlist Your Course</v-card-title>
              <v-card-text class="text--primary my-card-text">
                <p class="text--secondary">Checking <span class="font-italic">Fall 2020</span> course availability every minute.</p>
                <div class="btn-wrapper">
                  <v-btn to="/Unwaitlist-Request" raised color="#016030" class="white--text">Start Checking</v-btn>
                </div>
              </v-card-text>
            </v-card>

            <v-card class="my-card">
              <v-card-title class="my-card-title">❌ Cancel A Request</v-card-title>
              <v-card-text class="text--primary my-card-text">
                <p class="text--secondary">If unwaitlist is checking a class you're not interested in anymore, bop over here to cancel it.</p>
                <div class="btn-wrapper">
                  <v-btn to="/Unwaitlist-Cancelation" outlined color="#016030">Stop Checking</v-btn>
                </div>
              </v-card-text>
            </v-card>
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


/* add/remove btn styles*/
.btn-wrapper {
  display: flex;
  justify-content: flex-end;
}


/* adds border movement to cards */
@media screen and (max-width: 1263px) {
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
      title: 'Register'
    }
  }
}
</script>

