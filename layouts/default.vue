<template>
  <div>
    <TopBar />
    <HeaderNavigation />
    <nuxt />
  </div>
</template>

<script>
import TopBar from '~/components/nav/TopBar';
import HeaderNavigation from '~/components/nav/HeaderNavigation';

export default {
  components: {
    TopBar,
    HeaderNavigation
  }
}
</script>

<style>
:root {
  --theme: #EE234F;
  --theme-light: #ff9aa9;
  --theme-dark: #8E0E33;
  --secondary: #00A877;
  --secondary-dark: #00684C;
  --secondary-light: #D3EDEB;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  color: #222;
  font-family: 'Inter UI var alt', sans-serif;
}

a {
  color: inherit;
}
</style>
