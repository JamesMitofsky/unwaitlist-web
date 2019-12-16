<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Join the Fam</h2>
        <p>
          You're barely treading water and we definitely saw your head bob under. Thank goodness our program is better at
          unwaitlisting people than Zac Efron is at pretending to be a life guard.
        </p>
        <v-layout justify-center wrap xs12 md6 lg4>
            <v-card class="my-card">
              <v-card-title class="my-card-title">✅ Unwaitlist Your Course</v-card-title>
              <v-card-text class="text--primary my-card-text">
                <p class="text--secondary">Have the system check course availability every hour.</p>
                <div class="btn-wrapper">
                  <v-btn to="/Unwaitlist-A-Class" raised color="#016030" class="white--text">Start Checking</v-btn>
                </div>
              </v-card-text>
            </v-card>

            <v-card class="my-card">
              <v-card-title class="my-card-title">❌ Remove Course from Unwaitlist</v-card-title>
              <v-card-text class="text--primary my-card-text">
                <p class="text--secondary">If you want to cancel the an unwaitlist request, just bop over here.</p>
                <div class="btn-wrapper">
                  <v-btn to="/unknown" outlined color="#016030">Stop Checking</v-btn>
                </div>
              </v-card-text>
            </v-card>
        </v-layout>
              <!-- <v-card class="my-card">
                <v-card-title class="my-card-title">One n' done ✅</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check one class every hour
                    for
                    <span class="font-weight-bold">$5</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$5</span>
                    </div>
                    <v-btn to="/unwaitlist-one-class" small tile class="amber white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>

            <v-flex class="my-flex" xs12 md6 lg4>
              <v-card class="my-card">
                <v-card-title class="my-card-title">Three's for bees 🐝</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check three classes every hour
                     for
                    <span class="font-weight-bold">$4</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$12</span>
                    </div>
                    <v-btn small tile class="amber white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>

            <v-flex class="my-flex" xs12 md6 lg4>
              <v-card class="my-card">
                <v-card-title class="my-card-title">Five to jive 💃</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check five classes every hour
                    for
                    <span class="font-weight-bold">$3</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$15</span>
                    </div>
                    <v-btn small tile class="amber white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card> -->
          

        <!-- <div class="title">
          ❗ For an additional $2 per package, you can upgrade to checks
          <span
            class="font-italic"
          >every minute</span>.
        </div> -->
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

/* .card-bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
} */


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
      title: 'Register'
    }
  }
}
</script>

