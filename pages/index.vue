<template>
  <div id='page'>
    <Hero />
    <MailingList />
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
import MailingList from '~/components/nav/MailingList';
export default {
  components: {
    Hero,
    Intro,
    WhatTheySay,
    Sponsors,
    MailingList
  }
}
</script>


