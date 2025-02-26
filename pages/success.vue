<template>
  <v-layout column>
    <v-card>
      <v-card-title>Request Submitted!</v-card-title>
      <v-card-text
        class="text--primary"
      >A confirmation receipt will be emailed soon. To finish up, just Venmo me the cost of the package you requested and I'll activate it on my end.</v-card-text>
      <div class="payment-methods">
        <a href="https://venmo.com/JamesMitofsky">Finish by paying through Venmo.</a>

        <a href="https://venmo.com/JamesMitofsky">
          <img class="venmo-code" src="../static/jamesVenmo.png" alt="Venmo QR Code" />
        </a>
      </div>
      <script
            async
            src="https://static-na.payments-amazon.com/OffAmazonPayments/us/sandbox/js/Widgets.js"
          ></script>
          <div
            data-ap-widget-type="expressPaymentButton"
            data-ap-signature="LEDkAz7ZPProiEa%2B2MboTAzc1IR8Owf87BbaX6kC%2FM8%3D"
            data-ap-seller-id="AI7X50X1F3K0H"
            data-ap-access-key="AKIAI6SDNUAZDUSL6FQQ"
            data-ap-lwa-client-id="amzn1.application-oa2-client.010359452bae48f4afce984eb29a3e32"
            data-ap-return-url="https://unwaitlist.io/amazon-success"
            data-ap-currency-code="USD"
            data-ap-amount="5"
            data-ap-note="testy test dis note, thanks"
            data-ap-shipping-address-required="false"
            data-ap-payment-action="AuthorizeAndCapture"
            color="DarkGray"
          ></div>
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