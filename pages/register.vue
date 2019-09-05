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
        <v-container fluid grid-list-xs pa-2>
          <v-layout justify-center wrap>
            <v-flex class="my-flex" xs12 md6 lg4>
              <v-card class="my-card">
                <v-card-title class="my-card-title">One n' done ✅</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check one class every hour for
                    <span class="font-weight-bold">$5</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$5</span>
                    </div>
                    <v-btn small class="light-blue darken-3 white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>
            <!--  -->
            <v-flex class="my-flex" xs12 md6 lg4>
              <v-card class="my-card">
                <v-card-title class="my-card-title">Three's for bees 🐝</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check three classes every hour for
                    <span class="font-weight-bold">$4</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$12</span>
                    </div>
                    <v-btn small class="light-blue darken-3 white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>
            <!--  -->

            <v-flex class="my-flex" xs12 md6 lg4>
              <v-card class="my-card">
                <v-card-title class="my-card-title">Five to jive 💃</v-card-title>

                <v-card-text class="text--primary my-card-text">
                  <div class="subtitle-1">
                    Check five classes every hour for
                    <span class="font-weight-bold">$3</span>
                    <span class="text--secondary">per class in a semester</span>
                  </div>
                  <div class="card-bottom">
                    <div class="total-cost">
                      <span class="font-weight-bold">Total:</span>
                      <span>$15</span>
                    </div>
                    <v-btn small class="light-blue darken-3 white--text select-package">Select</v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

        <div class="title">
          ❗ For an additional $2 per package, you can upgrade to checks
          <span
            class="font-italic"
          >every minute</span>.
        </div>
      </div>
    </v-flex>
  </v-layout>
</template>

<style>
/* PURCHASE RELATED STYLES ------------------------------------------------ */

/* package card styles */
.my-flex {
  display: flex;
}

.my-card {
  flex: 1 1 auto;
  margin: 10px;
}

.my-card .my-card-title {
  font-weight: bold;
}


/* bottom of card styles */
.card-bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
}



div.card-bottom .v-btn.select-package.select-package {
  background-color: rgb(37, 106, 255);
}


/* adds border movement to cards */
@media screen and (max-width: 960px) {
  .v-card.v-card.v-card {
    border-left: 3px solid #2c769b;
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

