<template>
  <v-layout justify-center align-center wrap>
    <v-flex xs12 sm10 xl7>
      <!--Section: Join the Fam-->
      <div id="join-the-fam" class="content-block">
        <h2>Start Checking Your Course</h2>
        <br />
        <v-layout justify-center wrap xs12 md6 lg4>
          <iframe
            src="https://docs.google.com/forms/d/e/1FAIpQLSfwEiIB7jQnAqv9RcDmuLHoNMPsBiAHxI5b0sBW7uwmDL5p8g/viewform?embedded=true"
            width="640"
            height="766"
            frameborder="0"
            marginheight="0"
            marginwidth="0"
          >Loading…</iframe>
        </v-layout>
      </div>
    </v-flex>
  </v-layout>
</template>

<style scoped>
/* PURCHASE RELATED STYLES ------------------------------------------------ */

/* package card styles */
.my-card {
  flex: 1 1 auto;
  margin: 10px;
  display: flex;
  flex-direction: column;
}

.my-card .my-card-title {
  font-weight: bold;
}

/* add/remove btn styles*/
.btn-wrapper {
  display: flex;
  justify-content: flex-end;
}

/* adds border movement to cards */
@media screen and (max-width: 960px) {
  .v-card.v-card.v-card {
    border-left: 3px solid #ffc107;
    border-top: none;
  }
}
</style>


<script>
export default {
  head() {
    return {
      title: 'Requests'
    }
  },

  mounted() {
    // takes google confirmation text and updates it with ducky image

    // fields = document.getElementsByTagName("form")
    // test = document.getElementById("join-the-fam")
    // console.log(test)

    // fields.each((i, field) => {
    //                 // find text of current field
    //                 let fieldText = $(field).text();
    //                 // if the field text is that of enrollment, assign the element location to var
    //                 if (fieldText == "Enrolled/Seats:") {
    //                     enrollmentField = field
    //                 } else if (fieldText == "CRN:") {
    //                     crnField = field
    //                 }
    //             })
    
      // const gFormResponse = document.getElementsByClassName("freebirdFormviewerViewResponseConfirmationMessage")[0]

      // if(gFormResponse.textContent.includes("Yup, yup, yup")) {
      //   gFormResponse.textContent = "";
        
      //   let image = document.createElement("IMG");
      //   image.setAttribute("src", "https://i.pinimg.com/originals/83/e9/23/83e9236e9d9649d099209adc74015075.jpg");
      //   image.setAttribute("width", "371");
      //   image.setAttribute("height", "291");
      //   gFormResponse.append(image)
    
  }
    
  
}


</script>