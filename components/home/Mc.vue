<template>
  <div id="mc" class="w">
    <h2>And your lovely hosts are...</h2>
    <div class="split">
      <img src="~/assets/speakers/mc.jpg" alt="Matt & Jess Rose" />
      <div class="copy">
        <p>Jess Rose is Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae asperiores odit, eius aperiam saepe sit.</p>
        <p>Matt Rose is Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae asperiores odit, eius aperiam saepe sit.</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#mc {
  border-top: 1px solid var(--secondary-light);
  border-bottom: 1px solid var(--secondary-light);
  padding-bottom: 4em;
  margin-bottom: 4em;
}
h2 {
  margin: 2em 0;
  text-align: center;
}
.split {
  display: grid;
  grid-template-columns: 200px auto;
  grid-gap: 2em;
  img {
    width: 100%;
  }
  .copy {
    display: flex;
    flex-direction: column;
    justify-content: center;
    p:not(:last-child) {
      margin-bottom: 1em;
    }
  }
}
@media screen and (max-width: 600px) {
  h2 {
    margin-bottom: 1em;
  }
  .split {
    grid-template-columns: 1fr !important;
    img {
      width: 60%;
      display: block;
      margin: 0 auto;
    }
    .copy {
      text-align: center;
    }
  }
}
</style>