<template>
  <div id="top-bar">
    <span class="dates">January 18 2020</span>
    <!-- <span class="dates">January 18 2020. Birmingham, UK.</span> -->
    <div class="meta">
      <n-link to='/sponsor'>Sponsor</n-link>
      <a href='mailto:ygt@underland.events'>Email Us</a>
      <a href="https://twitter.com/search?q=%23YouGotThisConf">#YouGotThisConf</a>
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
  @media screen and (max-width: 800px) {
    display: none;
  }
}

</style>
