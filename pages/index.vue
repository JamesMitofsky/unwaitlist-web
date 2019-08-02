<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 md8 xl7>
      <div id="philosophy" class="content-block">
        <!--Section: Our Philosophy-->
        <div id="phil-header-container">
          <h2>Philosophy: No More Waiting*</h2>
          <p class="text-right text--secondary">*Well, still, actually, probably wait a little</p>
        </div>
        <p>
          Guaranteeing a spot during class sign-up is hard. Whether it's struggling to beat hoards of students at the crack of dawn or just realizing a little late which classes interest you,
          <span
            class="italics"
          >unwaitlist</span> can help.
        </p>

        <v-card>
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
      </div>
    </v-flex>
  </v-layout>
</template>

<style>


/* PHIL RELATED STYLES -------------------------------------------------- */

/* philosophy header grouping */
#phil-header-container {
  max-width: fit-content;
}
#phil-header-container p {
  font-size: 12px;
}
</style>

