<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <div class="content-block">
        <h2>Wutz Gud</h2>
        <div class="contact-wrapper">
            <img
              class="portrait"
              src="../assets/corporate_cup_walk.jpg"
              alt="Just a picture of little me boppin' around."
            />
            <v-card class="card">
              <v-card-text class="text--primary">
                Hi there, my name is James Tedesco and I'm a sophomore at the University of Vermont majoring in Political Science.
                I spend my free time eating fried ice cream, juggling, and making City Market trips just for the spectacle.
                Rather than give up procrastinating, I just leaned into knowing I'd realize too late which classes I wanted.
              </v-card-text>
              <v-card-text class="text--primary">
                Feel free to bop me at
                <a href="mailto:jtedesco@uvm.edu">jtedesco@uvm.edu</a>.
              </v-card-text>
            </v-card>
        </div>
      </div>
    </v-flex>
  </v-layout>
</template>

<style scoped>
/* when elements share width, add margin */
@media screen and (min-width: 900px) {
  .card {
    margin-left: 10px;
  }
}


@media screen and (max-width: 900px) {
  /* moves border to side of card when items become stacked */
  .v-card.v-card.v-card {
    border-left: 3px solid #FFC107;
    border-top: none;
    margin: 10px;
    max-width: 367px;
  }
  /* tells page elements to stack */
  .contact-wrapper {
    flex-direction: column;
    align-items: center;
  }
}

/* treat all main page items as flex */
.contact-wrapper {
  display: flex;
}

/* give picture radius of cards and set width properties */
.portrait {
  width: 94%;
  max-width: 367px;
  border-radius: 4px;
}
</style>

<script>
export default {
  head() {
    return {
      title: 'Contact'
    }
  }
}
</script>