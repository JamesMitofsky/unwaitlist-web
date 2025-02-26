<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <div class="content-block">
        <h1 class="fun-headers">No waitlist for these dms</h1>
        <div class="contact-wrapper">
          <img
            class="portrait"
            src="../assets/corporate_cup_walk.jpg"
            alt="Just me walking the corporate cup with my brothers' dad."
          />
          <v-card class="card indent-paragraph-children">
            <v-card-text class="text--primary">
              <p>
                Hi there, my name is James Mitofsky and I'm a sophomore at the University of Vermont majoring in Political Science.
                I spend my free time eating fried ice cream, playing music, and walking to City Market just for the spectacle.
                This project was born from an audacious degree of procrastination, but given its dependence on hope,
                I devote this to Obama the Redeemer.
              </p>
            </v-card-text>
            <v-card-text class="text--primary">
              <p class="no-indent">
                Feel free to bop me on
                <a
                  target="_blank"
                  href="https://twitter.com/JamesMitofsky802"
                >Twitter</a>.
              </p>
            </v-card-text>
            <v-card-text>
              <style>
  .bmc-button img {
    width: 35px !important;
    margin-bottom: 1px !important;
    box-shadow: none !important;
    border: none !important;
    vertical-align: middle !important;
  }
  .bmc-button {
    padding: 7px 10px 7px 10px !important;
    line-height: 35px !important;
    height: 51px !important;
    min-width: 217px !important;
    text-decoration: none !important;
    display: inline-flex !important;
    color: #ffffff !important;
    background-color: #ff813f !important;
    border-radius: 5px !important;
    border: 1px solid transparent !important;
    padding: 7px 10px 7px 10px !important;
    font-size: 28px !important;
    letter-spacing: 0.6px !important;
    box-shadow: 0px 1px 2px rgba(190, 190, 190, 0.5) !important;
    -webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
    margin: 0 auto !important;
    font-family: 'Cookie', cursive !important;
    -webkit-box-sizing: border-box !important;
    box-sizing: border-box !important;
    -o-transition: 0.3s all linear !important;
    -webkit-transition: 0.3s all linear !important;
    -moz-transition: 0.3s all linear !important;
    -ms-transition: 0.3s all linear !important;
    transition: 0.3s all linear !important;
  }
  .bmc-button:hover,
  .bmc-button:active,
  .bmc-button:focus {
    -webkit-box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
    text-decoration: none !important;
    box-shadow: 0px 1px 2px 2px rgba(190, 190, 190, 0.5) !important;
    opacity: 0.85 !important;
    color: #ffffff !important;
  }
              </style>
              <link href="https://fonts.googleapis.com/css?family=Cookie" rel="stylesheet" />
              <a
                class="bmc-button"
                target="_blank"
                href="https://www.buymeacoffee.com/JamesMitofsky"
              >
                <img
                  src="https://cdn.buymeacoffee.com/buttons/bmc-new-btn-logo.svg"
                  alt="Buy me a coffee"
                />
                <span style="margin-left:15px;font-size:28px !important;">Buy me a coffee</span>
              </a>
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
    border-left: 3px solid #ffc107;
    border-top: none;
    margin: 10px;
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
  width: 72vw;
  border-radius: 4px;
  object-fit: contain;
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