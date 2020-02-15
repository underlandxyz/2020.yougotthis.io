<template>
  <div>
    <TopBar />
    <HeaderNavigation />
    <nuxt />
    <!-- <MailingList /> -->
    <Underland />
  </div>
</template>

<script>
import TopBar from '~/components/nav/TopBar';
import HeaderNavigation from '~/components/nav/HeaderNavigation';
import MailingList from '~/components/nav/MailingList';
import Underland from '~/components/nav/Underland';

export default {
  components: {
    TopBar,
    HeaderNavigation,
    MailingList,
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
  --dark: #3A4B57;
  --mid: #939da4;
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
  max-width: 960px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 1em;
  padding-right: 1em;
  display: block;
}
</style>
