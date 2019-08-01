<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 md8 xl7>
      <div class="content-block">
        <!--Section: Our Philosophy-->
        <div id="phil-header-container">
          <h2>Philosophy: No More Waiting*</h2>
          <p class="text-right text--secondary">*Well, still, actually, probably wait a little</p>
        </div>
        <p>
          Guaranteeing a spot during class sign-up is hard. Whether it's beating hoards of students at the crack of dawn or just realizing a little late which classes interest you,
          <span
            class="italics"
          >unwaitlist can help</span>.
        </p>
      </div>

      <v-card class="content-block">
        <v-card-title>How does it work?</v-card-title>
        <v-card-text class="text--primary">
          <p>
            UVM's course registration system allows students to sign up at their leisure, but if a class is booked, you can request to be placed on the waitlist. Unfortunately,
            this waitlist might as well be quilled parchment - it has no connection to the registration portal. This means even if you were first on the waitlist, as soon as
            there's availablity in the class, absolutely anyone can take that spot.
          </p>
          <p>Unwaitlist checks the enrollment status of a given class at an assignable interval (i.e. every minute, hour, or 525,600 minutes), evaluates if there is an opening, and then if apppropriate, sends an email and calls you right away.</p>
        </v-card-text>
      </v-card>

      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Our Packages</h2>
        <v-card>
          <v-card-title>Star Student<span class="package-count">&nbsp;(1)</span></v-card-title>
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
          <v-card-title>Shoot ma goot<span class="package-count">&nbsp;(3)</span></v-card-title>
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
          <v-card-title>Delinquint<span class="package-count">&nbsp;(5)</span></v-card-title>
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
/* relevant global style */
.content-block {
  margin-bottom: 45px;
}

/* PHIL RELATED STYLES -------------------------------------------------- */

/* philosophy header grouping */
#phil-header-container {
  max-width: fit-content;
}
#phil-header-container p {
  font-size: 12px;
}

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

