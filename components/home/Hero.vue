<template>
  <div id='hero'>
    <div class="copy">
      <h1>An affordable one day conference for early-career developers.</h1>
      <h2>We're back for the second year to highlight the non-technical skills needed for a happy, healthy work life.</h2>
      <h3>January 18 2020</h3>
      <div class="topics">
        <img src="~/assets/site/topics-1.png" alt="">
        <img src="~/assets/site/topics-2.png" alt="">
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
    img {
      width: 100%;
      margin-top: 2em;
    }
    .topics {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 1em;
    }
  }
  h1 {
    font-size: 2.5em;
  }
  h2 {
    font-size: 1.5em;
    margin-top: 1em;
    margin-bottom: 0.5em;
    font-weight: normal;
  }
  h3 {
    font-weight: normal;
    margin-top: 1.5rem;
  }
  .img {
    img {
      height: 30em;
    }
  }
  @media screen and (max-width: 1000px) {
    flex-direction: column-reverse;
    .copy {
      text-align: center;
      padding-right: 0;
      h1 {
        font-size: 1.5em;
      }
      h2 {
        font-size: 1.25em;
        font-weight: normal;
      }
      .topics {
        grid-template-columns: 1fr;
        grid-gap: 0;
        margin-top: 1em;
        img {
          margin-bottom: 0;
          margin-top: 1em;
        }
      }
    }
    .img img {
      height: 10em;
      margin-bottom: 1em;
    }
  }
  @media screen and (max-width: 500px) {
    .copy .topics {
      display: none;
    }
  }
}
</style>
