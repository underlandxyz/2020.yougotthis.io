<template>
  <div id='mailing-list'>
    <form action="https://xyz.us18.list-manage.com/subscribe/post?u=434691fcaa2096849818903d2&amp;id=51fe5c8dd3" method="post"
      id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate w" target="_blank" novalidate>
      <label for="mce-EMAIL">Get updates</label>
      <input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL" placeholder="Email address">
      <input type="submit" value="Register" name="subscribe" id="mc-embedded-subscribe" class="button">
      <div style="position: absolute; left: -5000px; top: 0; pointer-events: none" aria-hidden="true">
        <input type="text" name="b_434691fcaa2096849818903d2_51fe5c8dd3" tabindex="-1" value="">
      </div>
    </form>
  </div>
</template>

<style lang="scss" scoped>
#mailing-list {
  background: var(--theme);
  form {
    margin-bottom: 0;
    padding: 1em;
    display: flex;
    align-items: center;
    label {
      margin-right: 1em;
      color: white;
    }
    input {
      padding: 0.75em;
      border: 0;
      -webkit-appearance: none;
    }
    input[type=email] {
      flex: 1;
      margin-right: 1em;
    }
    input[type=submit] {
      background: white;
    }
    @media screen and (max-width: 800px) {
      flex-direction: column;
      label, input {
        width: 100%;
        margin-left: 0 !important;
        margin-right: 0 !important;
      }
      label {
        text-align: center;
      }
      input {
        margin-top: 1em;
      }
    }
  }
}
</style>
