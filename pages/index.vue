<template>
  <div id='page'>
    <Hero />
    <Intro />
    <WhatTheySay />
  </div>
</template>

<script>
import Hero from '~/components/home/Hero';
import Intro from '~/components/home/Intro';
import WhatTheySay from '~/components/home/WhatTheySay';
export default {
  components: {
    Hero,
    Intro,
    WhatTheySay
  }
}
</script>


