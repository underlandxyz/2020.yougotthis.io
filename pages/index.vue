<template>
  <div id='page'>
    <Hero />
    <Intro />
    <Sponsors />
    <WhatTheySay />
  </div>
</template>

<script>
import Hero from '~/components/home/Hero';
import Intro from '~/components/home/Intro';
import Sponsors from '~/components/home/Sponsors';
import WhatTheySay from '~/components/home/WhatTheySay';
export default {
  components: {
    Hero,
    Intro,
    WhatTheySay,
    Sponsors
  }
}
</script>


