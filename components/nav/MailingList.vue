<template>
  <div id='mailing-list'>
    <form @submit.prevent='submit'>
      <label for="first">Register to the Underland Events mailing list for updates</label>
      <div class="inputs" v-if="!successful">
        <input v-model='first' type="text" id='first' placeholder='First Name' required>
        <input v-model='last' type="text" id='last' placeholder='Last Name' required>
        <input v-model='email' type="email" id='email' placeholder='Email Address' required>
        <input type="submit" value='Subscribe'>
      </div>
      <p v-else>Successfully subscribed</p>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      first: '',
      last: '',
      email: '',
      successful: false
    }
  },
  methods: {
    submit() {
      const { first, last, email } = this;
      this.$axios({
        method: 'POST',
        url: 'https://2020.yougotthis.io/.netlify/functions/mailing-list',
        data: { first, last, email }
      }).then(() => {
        this.successful = true;
      })
    }
  }
}
</script>

<style lang="scss" scoped>
#mailing-list {
  background: var(--theme);
  text-align: center;
  padding: 1em;
  label {
    color: white;
    margin-bottom: 0.25em;
    display: block;
  }
  input {
    padding: 0.75em;
    -webkit-appearance: none;
    border: 0;
    margin-top: 0.5em;
    &[type=submit] {
      background: white;
    }
  }
  p {
    margin-top: 0.5em;
    color: white;
  }
  @media screen and (max-width: 800px) {
    input {
      display: block;
      width: 100%;
    }
  }
}
</style>
