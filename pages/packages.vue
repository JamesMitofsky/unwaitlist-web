<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 md8 xl7>
      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Join the Fam</h2>
        <p>
          You're barely treading water and we definitely saw your head bob under. Thank goodness our program is better at
          unwaitlisting people than Zac Efron is at pretending to be a life guard.
        </p>

        <v-layout justify-center wrap>
          <v-flex xs12 md6>
            <v-card class="my-card">
              <v-card-title class="my-card-title">One n' done ✅</v-card-title>

              <v-card-text class="text--primary my-card-text">
                <div class="subtitle-1">Check one class every hour for $18</div>
                <div class="total-cost">
                  <span class="font-weight-bold">Total:</span>
                  <span>$18</span>
                </div>
              </v-card-text>
            </v-card>
          </v-flex>

          <v-flex xs12 md6>
            <v-card class="my-card">
              <v-card-title class="my-card-title">Three's for bees 🐝</v-card-title>

              <v-card-text class="text--primary my-card-text">
                <div class="subtitle-1">Check three classes every hour for $16</div>
                <span class="text--secondary">Per class</span>
                <div class="total-cost">
                  <span class="font-weight-bold">Total:</span>
                  <span>$48</span>
                </div>
              </v-card-text>
            </v-card>
          </v-flex>
          <!--  -->

          <v-flex xs12 md6>
            <v-card class="my-card">
              <v-card-title class="my-card-title">Five to jive 💃</v-card-title>

              <v-card-text class="text--primary my-card-text">
                <div class="subtitle-1">Check five classes every hour for $13</div>
                <span class="text--secondary">Per class</span>
                <div class="total-cost">
                  <span class="font-weight-bold">Total:</span>
                  <span>$65</span>
                </div>
              </v-card-text>
            </v-card>
          </v-flex>
        </v-layout>

        <div class="title">
          ❗ For an additional $10 on any package, you can upgrade to a course check
          <span class="font-italic">every minute</span>.
        </div>
      </div>
    </v-flex>
  </v-layout>
</template>

<style>
/* PURCHASE RELATED STYLES ------------------------------------------------ */

/* package card styles */
.card-container {
  display: flex;
  flex: wrap;
}

.my-card {
  display: flex;
  flex-direction: column;
  margin: 10px;
}

.my-card .my-card-title {
  font-weight: bold;
}

.total-cost {
  margin: 10px;
}

/* pill styled price listings */
/* .pill {
  box-shadow: grey 1px 1px 4px 0px;
  border-radius: 3px;
  white-space: nowrap;
  padding: 2px;
  margin: 3px;
}
.pill.one-min {
  background-color: azure;
}
.pill.sixty-mins {
  background-color: rgb(255, 228, 228);
} */

.package-count {
  color: lightslategray;
}
</style>

