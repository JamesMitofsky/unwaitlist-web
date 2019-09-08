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
        onload="if(submitted)  {window.location='success';}"
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
          <div class="form-subset input-block">
            <label for="firstName">First Name</label>
            <input id="firstName"
              placeholder="Gary"
              name="entry.175684321"
              type="text"
              autocomplete="email"
              required
            />
          </div>

          <div class="form-subset input-block">
            <label for="lastName">Last Name</label>
            <input id="lastName" placeholder="Derr" name="entry.1110633439" type="text" required />
          </div>

          <div class="form-subset input-block">
            <label for="emailAddress">Email</label>
            <input
              id="emailAddress"
              placeholder="Gary.Derr@email.com"
              name="entry.1057850542"
              type="email"
              autocomplete="email"
              required
            />
          </div>

          <div class="form-subset input-block">
            <label for="cellPhone">Cell Phone</label>
            <input
              id="cellPhone"
              placeholder="(802) 867-5309"
              name="entry.122122566"
              type="tel"
              required
            />
          </div>

          <div class="form-subset input-block">
            <label for="crnInput">CRN</label>
            <!-- Max nums: https://stackoverflow.com/a/50442323/5395435 -->
            <input
            id="crnInput"
              placeholder="95377"
              name="entry.232057564"
              type="number"
              pattern="/^-?\d+\.?\d*$/"
              onKeyPress="if(this.value.length==5) return false;"
              required
            />
          </div>

          <div class="form-subset">
            <v-btn class="light-blue darken-3 white--text" id="submit-button" type="submit" value="Submit">Submit</v-btn>
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

input {
  padding: 0px 3px;
  background-color: white;
  box-shadow: hsl(204, 27%, 56%) 1px 1px 5px 0px;
}

#submit-button {
  transition: all .2s;
  cursor: pointer
}
</style>