<template>
  <div id="top-bar">
    <span class="dates">January 18 2020. Birmingham, UK.</span>
    <div class="meta">
      <n-link to='/contact'>Contact</n-link>
      <n-link to='/sponsor'>Sponsor</n-link>
      <a href="">#YouGotThisConf</a>
      <a href='https://underland.events'>Underland Events</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#top-bar {
  background: var(--theme-dark);
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 1em;
  font-size: 0.8em;
  * {
    color: white;
  }
  .meta a {
    margin-left: 1em;
    text-decoration: none;
  }
  @media screen and (max-width: 1000px) {
    display: none;
  }
}

</style>
