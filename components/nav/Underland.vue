<template>
  <div id="underland">
    <a class="w" href="https://twitter.com/underlandevents">
      <img src="~/assets/brand/underland-events.svg" alt="Underland Events" />
      <p>Organised by Underland Events - the developer events company.</p>
    </a>
    <span class="w conduct"
      ><a href="https://www.techevents.online/" target="_blank"
        >As featured on TechEvents.online</a
      ></span
    >
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
  span,
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
