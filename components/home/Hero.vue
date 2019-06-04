<template>
  <div id='hero'>
    <div class="copy">
      <h1>An afforable one-day conference for early-career developers.</h1>
      <h2>Covering the non-technical skills needed for a happy, healthy work life.</h2>
      <img src="~/assets/site/topics.png" alt="">
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
