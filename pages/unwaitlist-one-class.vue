<template>
  <v-layout align-center column>
    <!-- Breadcrumbs here -->
    <v-breadcrumbs class="breadcrumbs" :items="items">
      <template v-slot:divider>
        <v-icon>mdi-chevron-right</v-icon>
      </template>
    </v-breadcrumbs>

    <v-layout column>
      <!-- Display package selection -->
      <v-card class="my-card">
        <v-card-title class="my-card-title">One n' done ✅</v-card-title>

        <v-card-text class="text--primary my-card-text">
          <div class="subtitle-1">
            Check one class every hour for
            <span class="font-weight-bold">$5</span>
            <span class="text--secondary">per class in a semester</span>
          </div>
          <div class="card-bottom">
            <div class="total-cost">
              <span class="font-weight-bold">Total:</span>
              <span>$5</span>
            </div>
          </div>
        </v-card-text>
      </v-card>

      <!-- Accessing gForms: https://blog.webjeda.com/google-form-customize/ -->
      <iframe
        name="hidden_iframe"
        id="hidden_iframe"
        style="display:none;"
        onload="if(submitted) {window.location='success';}"
      ></iframe>

      <v-card class="my-card form-card">
        <v-card-title class="my-card-title">Unwaitlist Your Class!</v-card-title>
        <form
          class="form"
          action="https://docs.google.com/forms/u/1/d/e/1FAIpQLSdL6QgGVjqsDvZsEx__yltIvMmzWdfCX4NHksRmbgC1JQOrYA/formResponse"
          method="post"
          target="hidden_iframe"
          onsubmit="submitted=true;"
          autocomplete="on"
        >
          <div class="form-subset">
            <label for="firstName">First Name</label>
            <input
              id="firstName"
              placeholder="e.g. Gary"
              name="entry.175684321"
              type="text"
              required
            />
          </div>

          <div class="form-subset">
            <label for="lastName">Last Name</label>
            <input
              id="lastName"
              placeholder="e.g. Derr"
              name="entry.1110633439"
              type="text"
              required
            />
          </div>

          <div class="form-subset">
            <div class="label-block">
              <label for="emailAddress">Email</label>
              <div class="help-tip">
                <p>Used to share important course changes in a readable, non-time-sensative way.</p>
              </div>
            </div>

            <input
              id="emailAddress"
              placeholder="e.g. Gary.Derr@email.com"
              name="entry.1057850542"
              type="email"
              autocomplete="email"
              required
            />
          </div>

          <div class="form-subset">
            <div class="label-block">
              <label for="cellPhone">Phone</label>
              <div class="help-tip">
                <p>Used to call you if your class opens up.</p>
              </div>
            </div>
            <input
              id="cellPhone"
              placeholder="e.g. (802) 867-5309"
              name="entry.122122566"
              type="tel"
              autocomplete="mobile"
              required
            />
          </div>

          <div class="form-subset">
            <label for="crnInput">CRN</label>
            <!-- Max nums: https://stackoverflow.com/a/50442323/5395435 -->
            <input
              id="crnInput"
              placeholder="e.g. 95377"
              name="entry.232057564"
              type="number"
              min="0"
              max="99999"
              required
            />
          </div>

          <div class="form-subset">
            <v-btn
              tile
              class="amber white--text"
              id="submit-button"
              type="submit"
              value="Submit"
            >Submit</v-btn>
          </div>
        </form>
      </v-card>
    </v-layout>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
      submitted: false,
      items: [
        {
          text: 'Home',
          to: '/'
        },
        {
          text: 'Register',
          to: '/register'
        },
        {
          text: "One n' Done",
          to: '/unwaitlist-one-class'
        }
      ]
    }
  }
}
</script>


<style scoped>
.breadcrumbs {
  align-self: flex-start;
}

.my-card {
  margin: 10px;
}

.form {
  padding: 10px 25px;
  display: flex;
  flex-direction: column;
  width: auto;
}

.form-subset {
  display: flex;
  flex-direction: column;
  margin: 10px;
  border-radius: 5px;
  padding: 4px;
}

.label-block {
  display: flex;
  justify-content: space-between;
}
.information-svg {
  width: 15px;
}
.info-text {
  background-color: rgb(255, 206, 214);
  width: 105px;
  display: block;
  position: absolute;
  right: 0;
  top: 0;
  padding: 3px;
  border-radius: 3px;
}
.information-svg:hover + .info-text {
  display: block;
}

input {
  padding: 0px 3px;
  background-color: white;
  box-shadow: #aeaa61 1px 1px 5px 0px;
}

#submit-button {
  transition: all 0.2s;
  cursor: pointer;
}

/* CSS grabbed from: https://tutorialzine.com/2014/07/css-inline-help-tips */
.help-tip {
  text-align: center;
  background-color: #bcdbea;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  line-height: 26px;
  cursor: default;
}

.help-tip:before {
  content: '?';
  font-weight: bold;
  color: #fff;
}

.help-tip:hover p {
  display: block;
  transform-origin: 100% 0%;

  -webkit-animation: fadeIn 0.3s ease-in-out;
  animation: fadeIn 0.3s ease-in-out;
}

.help-tip p {
  /* The tooltip */
  display: none;
  text-align: left;
  background-color: #1e2021;
  padding: 12px;
  width: 300px;
  position: absolute;
  border-radius: 3px;
  box-shadow: 1px 1px 1px rgba(0, 0, 0, 0.2);
  right: -4px;
  color: #fff;
  font-size: 13px;
  line-height: 1.4;
}

.help-tip p:before {
  /* The pointer of the tooltip */
  position: absolute;
  content: '';
  width: 0;
  height: 0;
  border: 6px solid transparent;
  border-bottom-color: #1e2021;
  right: 48px;
  top: -12px;
}

.help-tip p:after {
  /* Prevents the tooltip from being hidden */
  width: 100%;
  height: 40px;
  content: '';
  position: absolute;
  top: -40px;
  left: 0;
}

/* CSS animation */

@-webkit-keyframes fadeIn {
  0% {
    opacity: 0;
    transform: scale(0.6);
  }

  100% {
    opacity: 100%;
    transform: scale(1);
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 100%;
  }
}
</style>