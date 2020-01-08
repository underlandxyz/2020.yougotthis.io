<template>
  <div id='hero'>
    <div class="copy">
      <h2>January 18 2020. Birmingham, UK.</h2>
      <h1>We're back! An affordable one day conference for early-career developers to talk about the non-technical skills needed for a happy, healthy work life.</h1>
      <div class="tickets">
        <a class='cta btn' href='https://www.eventbrite.co.uk/e/you-got-this-2020-tickets-77737122827'>Buy Tickets</a>
        <n-link to='/schedule' class='cta btn minor'>Schedule</n-link>
      </div>
    </div>
    <div class="img">
      <img src="~/assets/brand/logo.png" alt="">
    </div>
  </div>
</template>

<style lang="scss" scoped>
#hero {
  display: flex;
  flex-direction: row;
  width: 100%;
  padding: 2em;
  align-items: center;
  .copy {
    padding-right: 2em;
  }
  h1 {
    font-size: 2em;
    margin: 1.5rem 0 1rem;
  }
  h2 {
    font-size: 1.25em;
    font-weight: normal;
  }
  .img {
    img {
      height: 30em;
    }
  }
  .cta.btn {
    background: var(--secondary);
    color: white;
    padding: 0.75em 1.5em;
    text-decoration: none;
    display: inline-block;
    margin-top: 1em;
    &.minor {
      background: var(--secondary-light);
      color: var(--dark);
    }
  }
  @media screen and (max-width: 1000px) {
    flex-direction: column-reverse;
    .copy {
      text-align: center;
      padding-right: 0;
      h1 {
        font-size: 1.25em;
        margin-top: 1em;
      }
      h2 {
        font-size: 1em;
        font-weight: normal;
        margin-top: 1em;
      }
    }
    .img img {
      height: 10em;
      margin-bottom: 1em;
    }
  }
}
</style>
