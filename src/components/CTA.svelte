<script>
  import { postData } from '../utils/postData'
  import { writable } from 'svelte/store'
  import axios from 'axios'

  let email = writable("");

  let submitForm = () => {
    // axios.post("https://tpeo-week-2-api.marshall.now.sh/api/send-email", {
    //   email: $email
    // }).then((res) => {
    //   console.log({res});
    // }).catch((err) => {
    //   console.error(err);
    // })
    alert("Submit!")
  }

</script>

<style lang="scss">
  @import "./GlobalStyle/theme.scss";

</style>

  <input name="email" bind:value={$email} />
  <button on:click={submitForm}>Send</button>
