<template>
  <div id="sponsors" class="w">
    <h2>Made possible by...</h2>
    <div class="logos">
      <a v-for="sponsor in sponsors" :key="sponsor.link" :href="sponsor.link">
        <img :src="require(`@/assets/sponsors/${sponsor.image}`)" :alt="sponsor.name" />
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
          name: 'GitHub',
          image: 'github.png',
          link: 'https://github.com/'
        },
        {
          name: 'Balsamiq',
          image: 'balsamiq.png',
          link: 'https://balsamiq.com/'
        },
        {
          name: 'Mozilla',
          image: 'mozilla.png',
          link: 'https://www.mozilla.org'
        },
        {
          name: 'Twilio',
          image: 'twilio.png',
          link: 'https://twilio.com/'
        },
        {
          name: 'Samsung Internet',
          image: 'samsung-internet.png',
          link: 'https://samsunginter.net/'
        },
        {
          name: 'DigitalOcean',
          image: 'digital-ocean.png',
          link: 'https://www.digitalocean.com/'
        },
        {
          name: 'Pusher',
          image: 'pusher.png',
          link: 'https://pusher.com/'
        },
        {
          name: 'Major League Hacking',
          image: 'mlh.png',
          link: 'https://mlh.io/'
        },
        {
          name: 'Auth0',
          image: 'auth0.png',
          link: 'https://auth0.com/'
        },
        {
          name: 'Fastprint',
          image: 'fastprint.png',
          link: 'https://www.fastprint.co.uk/'
        },
        {
          name: 'Proactive',
          image: 'proactive.png',
          link: 'http://proactive.uk.net'
        },
        {
          name: '',
          image: 'you.png',
          link:
            'mailto:ygt@eunderland.events?subject=You Got This 2020 Sponsorship'
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
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 1.5em;
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
