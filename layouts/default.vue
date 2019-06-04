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
  --theme: #AD0010;
  --theme-light: #FF3E5A;
  --theme-dark: #6E0003;
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
