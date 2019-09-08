<template>
  <v-layout column>
    <v-card>
      <v-card-title>Request Submitted!</v-card-title>
      <v-card-text
        class="text--primary"
      >A confirmation receipt will be emailed soon. To finish up, just Venmo me the cost of the package you requested and I'll activate it on my end.</v-card-text>
      <div class="payment-methods">
        <a href="https://venmo.com/JamesTedesco">Finish by paying through Venmo.</a>

        <a href="https://venmo.com/JamesTedesco">
          <img class="venmo-code" src="../static/jamesVenmo.png" alt="Venmo QR Code" />
        </a>
      </div>
    </v-card>
  </v-layout>
</template>

<style scoped>
.venmo-code {
  max-width: 200px;
}

.payment-methods {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>