<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <div id="philosophy" class="content-block">
        <!--Section: Our Philosophy-->
        <div id="phil-header-container">
          <h2>Philosophy: No More Waiting*</h2>
          <p class="text-right text--secondary">*Well, still, actually, probably a little</p>
        </div>
        <p>
          Guaranteeing a spot during class sign-up is hard. Whether it's struggling to beat hoards of students at the crack of dawn or just realizing a little late which classes interest you,
          <span
            class="font-italic"
          >unwaitlist</span> can help.
        </p>

        <v-card>
          <v-card-title>TL;DR</v-card-title>
          <v-card-text class="text--primary">UVM students, get notified when class is open.</v-card-text>
        </v-card>

        <v-card>
          <v-card-title>What's the Gist?</v-card-title>
          <v-card-text class="text--primary">
            <p>
              UVM's course registration system allows students to sign up at their leisure, but if a class is booked, you can request to be placed on the waitlist. Unfortunately,
              this waitlist might as well be quilled parchment - it has no connection to the registration portal. This means as soon as the class has an opening,
              <span
                class="font-italic"
              >even if you were first on the waitlist</span>, absolutely anyone can take that spot.
            </p>
            <p>
              Solving for this,
              <span class="font-italic">unwaitlist</span> checks the enrollment status of a given class at an assignable interval (i.e. every minute, hour, or 525,600 minutes), evaluates if there is an opening, and then if apppropriate, sends an email and calls you right away.
            </p>
          </v-card-text>
        </v-card>
      </div>
    </v-flex>
  </v-layout>
</template>

<style scoped>

.v-card.v-card.v-card {
  border-left: 3px solid #FFC107;
  border-top: none;
}

/* philosophy header grouping */
#phil-header-container {
  max-width: fit-content;
}
#phil-header-container p {
  font-size: 12px;
}

.free-service {
  display: flex;
  align-items: end;
  flex-direction: column;
}

.free-service .v-card-title .img {
  display: flex;
}

.v-card {
  margin: 10px 0;
}
</style>

<script>
export default {
  head() {
    return {
      title: 'Home'
    }
  }
}
</script>

