<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 md8 xl7>
      <div class="content-block">
        <h2>Contact</h2>
        <v-card class="card">
          <div>
            <v-flex>
              <img
                class="portrait"
                src="../assets/little-james.jpg"
                alt="Just a picture of little me boppin' around."
              />
            </v-flex>
            <v-flex>
              <v-card-text class="text--primary">
                Hi there, my name is James Tedesco and I'm a sophmore at the University of Vermont.
                I'm a Political Science major and I spend my free time making countless trips to City Market just for the spectacle.
                This began as a personal project but scaling it out has been a blast.
              </v-card-text>
              <v-card-text class="text--primary">
                Feel free to bop me at
                <a
                  href="mailto:jtedesco@uvm.edu"
                >jtedesco@uvm.edu</a>.
              </v-card-text>
            </v-flex>
          </div>
        </v-card>
      </div>
    </v-flex>
  </v-layout>
</template>

<style>
.card {
  overflow: hidden;
}

.portrait {
  max-width: 400px;
}
</style>

