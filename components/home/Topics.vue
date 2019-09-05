<template>
  <div id='topics' class="w">
    <h2>We talk about subjects such as...</h2>
    <div class="topics">
      <img src="~/assets/site/topics-1.png" alt="">
      <img src="~/assets/site/topics-2.png" alt="">
    </div>
  </div>
</template>

<style lang="scss" scoped>
h2 {
  text-align: center;
}
img {
  width: 100%;
  margin-top: 1em;
}
.topics {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 1em;
  margin-bottom: 4em;
}
@media screen and (max-width: 1000px) {
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
@media screen and (max-width: 500px) {
  #topics {
    display: none;
  }
  .copy .topics {
    display: none;
  }
}
</style>