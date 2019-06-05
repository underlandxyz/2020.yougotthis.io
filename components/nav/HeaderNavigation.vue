<template>
  <div id='header-navigation'>
    <nav>
      <n-link to='/' class='brand'>
        <h1>You Got This!</h1>
      </n-link>
      <div class="inner">
        <n-link v-for='link in nav' :key='link.path' :to='link.path' :class='link.class'>{{link.text}}</n-link>
      </div>
    </nav>
    <!-- <n-link to='/talk' class="cta btn apply">Submit a talk</n-link> -->
    <div id="mob-menu">
      <nav>
        <n-link v-for='link in mobNav' :key='link.path' :to='link.path'>{{link.text}}</n-link>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showNav: false,
      nav: [
        // { text: 'Schedule', path: '/schedule', class:'bold' },
        // { text: 'Venue', path: '/venue', class:'minor' },
        { text: 'Inclusion Programme', path: '/inclusion', class:'minor' },
        // { text: 'Food', path: '/food', class:'bold' },
        { text: 'Code of Conduct', path: '/conduct', class:'minor' }
      ],
      mobNav: [
        { text: 'Inclusion', path: '/inclusion' },
        // { text: 'Conduct', path: '/conduct' },
        // { text: 'Sponsor', path: '/sponsor' },
        // { text: 'Submit a talk', path: '/talk' }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#header-navigation {
  background: var(--theme);
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  font-size: 0.8em;
  nav {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    a {
      text-decoration: none;
      padding: 1.5em 1.25em 1.3em;
      display: inline-block;
      border-right: 1px solid rgba(229, 229, 229, 0.2);
      color: white;
      border-bottom: 4px solid transparent;
      &.brand {
        h1 {
          font-size: 1em;
          text-transform: uppercase;
        }
      }
      &.bold {
        text-transform: uppercase;
        font-weight: bold;
      }
    }
    .inner .nuxt-link-active {
      border-bottom-color: var(--theme-dark);
    }
  }
  .cta {
    background: var(--secondary);
    color: white;
    display: flex;
    align-items: center;
    padding: 1.5em;
    text-transform: uppercase;
    text-decoration: none;
    font-weight: bold;
  }
  #mob-menu {
    display: none;
  }
  @media screen and (max-width: 800px) {
    .inner,
    .cta {
      display: none;
    }
    #mob-menu {
      display: block;
      nav a {
        border-right: 0;
      }
    }
  }
}
</style>
