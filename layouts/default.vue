<template>
  <div>
    <TopBar />
    <HeaderNavigation />
    <nuxt />
    <Footer />
    <Underland />
  </div>
</template>

<script>
import TopBar from '~/components/nav/TopBar';
import HeaderNavigation from '~/components/nav/HeaderNavigation';
import Footer from '~/components/nav/Footer';
import Underland from '~/components/nav/Underland';

export default {
  components: {
    TopBar,
    HeaderNavigation,
    Footer,
    Underland
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
  --dark: #161B24;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  color: var(--dark);
  font-family: 'Inter UI var alt', sans-serif;
  line-height: 1.5;
}

a {
  color: inherit;
}

.w {
  max-width: 860px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 1em;
  padding-right: 1em;
  display: block;
}
</style>
