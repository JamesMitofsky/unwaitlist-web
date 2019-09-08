<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <div class="content-block">
        <h2>Contact</h2>
        <v-layout wrap>
          <v-flex xs12 sm6>
            <img
              class="portrait"
              src="../assets/little-james.jpg"
              alt="Just a picture of little me boppin' around."
            />
          </v-flex>
          <v-flex xs12 sm6>
            <v-card class="card">
              <v-card-text class="text--primary">
                Hi there, my name is James Tedesco and I'm a sophomore at the University of Vermont majoring in Political Science.
                I spend my free time eating fried ice cream, juggling, and making trips to City Market just for the spectacle.
                This project began as a way to compensate for my own laziness and I hope the spirit of that lives on through others.
              </v-card-text>
              <v-card-text class="text--primary">
                Feel free to bop me at
                <a href="mailto:jtedesco@uvm.edu">jtedesco@uvm.edu</a>.
              </v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
      </div>
    </v-flex>
  </v-layout>
</template>

<style>

/* when elements share width, add margin */
@media screen and (min-width: 600px) {
  .card{
    margin-left: 10px;
  }
}

/* when elements are stacked, move border highlight to side */
@media screen and (max-width: 600px) {
  .v-card.v-card.v-card {
  border-left: 3px solid #2C769B;
  border-top: none;
  }
}

.portrait {
  width: 100%;
  max-width: 600px;
}
</style>

<script>
export default {
  head () {
    return {
      title: "Contact",
    }
  }
}
</script>