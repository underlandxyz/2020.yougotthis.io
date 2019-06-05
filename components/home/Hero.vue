<template>
  <div id='hero'>
    <div class="copy">
      <h1>An afforable one day conference for early-career developers.</h1>
      <h2>We're back for the second year to highlight the non-technical skills needed for a happy, healthy work life.</h2>
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
  border-bottom: 4px solid var(--dark);
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
    font-size: 3em;
  }
  h2 {
    font-size: 2em;
    margin-top: 1em;
  }
  .img {
    img {
      height: 30em;
    }
  }
}
</style>
