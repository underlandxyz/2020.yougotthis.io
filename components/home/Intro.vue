<template>
  <div id="intro" class='w'>
    <h2>You Got This is for...</h2>
    <div class="roles">
      <div class="role">
        <img src="https://placehold.it/500x500" alt="">
        <p>Folks looking to soon get their first developer role</p>
      </div>
      <div class="role">
        <img src="https://placehold.it/500x500" alt="">
        <p>Junior devs looking to skill-up and grow professionally</p>
      </div>
      <div class="role">
        <img src="https://placehold.it/500x500" alt="">
        <p>Managers wanting to better support their team</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
h2 {
  margin: 2em 0;
  text-align: center;
}
.roles {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 2em;
  margin-bottom: 2em;
  img {
    width: 100%;
    display: none;
  }
  p {
    margin: 1em 0;
    text-align: center;
  }
}
@media screen and (max-width: 600px) {
  .roles {
    grid-template-columns: 1fr;
    img {
      width: 50%;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
  }
}
</style>