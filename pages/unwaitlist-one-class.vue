<template>
<v-layout>
    <iframe name="hidden_iframe" id="hidden_iframe" style="display:none;" onload="if(submitted)  {window.location='success';}"></iframe>
  <form
    class="form"
    action="https://docs.google.com/forms/u/1/d/e/1FAIpQLSdL6QgGVjqsDvZsEx__yltIvMmzWdfCX4NHksRmbgC1JQOrYA/formResponse" method="post" target="hidden_iframe"
    onsubmit="submitted=true;">
    <label>Email</label>
    <input name="entry.1057850542" type="email" required />

    <label>First Name</label>
    <input name="entry.175684321" type="text" required />

    <label>Last Name</label>
    <input name="entry.1110633439" type="text" required />

    <label>CRN</label>
    <input name="entry.232057564" type="number" required />

    <input
        type="submit" value="Send" />
  </form>

  <button ></button>

  <div id="confirmation-block">{{ submitted }}</div>
  </v-layout>
</template>


<script>
export default {
    data() {
        return { submitted: false }
    }
}
</script>