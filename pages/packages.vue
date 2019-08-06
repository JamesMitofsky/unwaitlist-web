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
                    <span class="font-weight-bold">$13</span>
                  </div>
                  <div class="total-cost">
                    <span class="font-weight-bold">Total:</span>
                    <span>$13</span>
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
                    <span class="font-weight-bold">$11</span>
                    <span class="text--secondary">per class</span>
                  </div>
                  <div class="total-cost">
                    <span class="font-weight-bold">Total:</span>
                    <span>$33</span>
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
                    <span class="font-weight-bold">$8</span>
                    <span class="text--secondary">per class</span>
                  </div>
                  <div class="total-cost">
                    <span class="font-weight-bold">Total:</span>
                    <span>$40</span>
                  </div>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

        <div class="title">
          ❗ For an additional $7 per class, you can upgrade for checks
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
  /* display: flex;
  flex-direction: column; */
  margin: 10px;
  flex: 1 1 auto;
}

.my-card .my-card-title {
  font-weight: bold;
}

.total-cost {
  margin: 10px;
}

.package-count {
  color: lightslategray;
}

@media screen and (max-width: 960px) {
  .v-card.v-card.v-card {
    border-left: 3px solid #2c769b;
    border-top: none;
  }
}
</style>


<script>
export default {
  head () {
    return {
      title: "Packages",
    }
  }
}
</script>

