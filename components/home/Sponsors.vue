<template>
  <div id='sponsors' class='w'>
    <h2>Made possible by...</h2>
    <div class="logos">
      <a v-for='sponsor in sponsors' :key='sponsor.link' :href="sponsor.link">
        <img :src="require(`@/assets/sponsors/${sponsor.image}`)" alt="">
      </a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sponsors: [
        {
          image: 'balsamiq.png',
          link: 'https://balsamiq.com/'
        },
        {
          image: 'twilio.png',
          link: 'https://twilio.com/'
        },
        {
          image: 'you.png',
          link: 'mailto:ygt@eunderland.events?subject=You Got This 2020 Sponsorship'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#sponsors {
  margin-bottom: 4rem;
}
h2 {
  text-align: center;
}
.logos {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 2em;
  margin-top: 1em;
}
img {
  width: 100%;
}
@media screen and (max-width: 600px) {
  .logos {
    grid-template-columns: 1fr 1fr;
  }
  .logos div {
    display: none;
  }
}
</style>
