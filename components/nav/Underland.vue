<template>
  <div id='underland'>
    <a class="w" href="https://underland.events">
      <img src="~/assets/brand/underland-events.svg" alt="Underland Events">
      <p>Organised by Underland Events - the developer events company.</p>
    </a>
    <n-link class='w conduct' to='/conduct'>Code of Conduct</n-link>
  </div>
</template>

<style lang="scss" scoped>
#underland {
  background: var(--theme-dark);
  padding-top: 2em;
  padding-bottom: 2em;
  text-align: center;
  img {
    height: 3em;
    margin-bottom: 1.5em;
  }
  a {
    color: white;
    text-decoration: none;
  }
  .conduct {
    font-size: 0.8em;
    margin-top: 1rem;
  }
}
</style>