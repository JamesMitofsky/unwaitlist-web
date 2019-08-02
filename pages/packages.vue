<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 md8 xl7>

      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Our Packages</h2>
        <v-card>
          <v-card-title>
            Star Student
            <span class="package-count">&nbsp;(1 class)</span>
          </v-card-title>
          <v-card-text class="text--primary">
            Today you're waiting for one class, tomorrow you'll be waiting for your self-loathing to pass, again. If you're looking for a quick way to buy your way out of this destructive pattern... wrong website. But in the meantime,
            we'll handle even your simple unwaitlist needs.
            <div class="price-block">
              Check
              <span class="italics">one class</span> every
              <span class="pill sixty-mins">hour for $60</span> or every
              <span class="pill one-min">minute for $100</span>.
            </div>
          </v-card-text>
        </v-card>

        <v-card>
          <v-card-title>
            Shoot ma goot
            <span class="package-count">&nbsp;(3 classes)</span>
          </v-card-title>
          <v-card-text class="text--primary">
            You're barely treading water and we definitely saw your head bob under. Thank goodness our program is as
            good at unwaitlisting people as Zac Efron is at pretending to be a life guard. Your odds look survivable, but we'll drop you a 15% break.
            <div class="price-block">
              Check
              <span class="italics">three classes</span> every
              <span class="pill sixty-mins">hour for $51 per class</span> or every
              <span class="pill one-min">minute for $85 per class</span>.
            </div>
          </v-card-text>
        </v-card>

        <v-card>
          <v-card-title>
            Delinquint
            <span class="package-count">&nbsp;(5 classes)</span>
          </v-card-title>
          <v-card-text class="text--primary">
            Duuudddeeee, yikes. Although this is a strange time to begin acknowledging responsibilities,
            we grant that it's better late than never. As some semblance of a consolation, we'll cut you a 30% discount.
            <div class="price-block">
              Check
              <span class="italics">five classes</span> every
              <span class="pill sixty-mins">hour for $42 per class</span> or every
              <span class="pill one-min">minute for $70 per class</span>.
            </div>
          </v-card-text>
        </v-card>
      </div>
    </v-flex>
  </v-layout>
</template>

<style>
/* PURCHASE RELATED STYLES ------------------------------------------------ */

/* pill styled price listings */
.pill {
  box-shadow: grey 1px 1px 4px 0px;
  border-radius: 3px;
  white-space: nowrap;
  padding: 2px;
}
.pill.one-min {
  background-color: azure;
}
.pill.sixty-mins {
  background-color: rgb(255, 228, 228);
}

.price-block {
  margin: 10px 0;
}

.package-count {
  color: lightslategray;
}
</style>

